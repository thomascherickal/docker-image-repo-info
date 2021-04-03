<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:10.1`](#mariadb101)
-	[`mariadb:10.1-bionic`](#mariadb101-bionic)
-	[`mariadb:10.1.48`](#mariadb10148)
-	[`mariadb:10.1.48-bionic`](#mariadb10148-bionic)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.2.37`](#mariadb10237)
-	[`mariadb:10.2.37-bionic`](#mariadb10237-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.3.28`](#mariadb10328)
-	[`mariadb:10.3.28-focal`](#mariadb10328-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.4.18`](#mariadb10418)
-	[`mariadb:10.4.18-focal`](#mariadb10418-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10.5.9`](#mariadb1059)
-	[`mariadb:10.5.9-focal`](#mariadb1059-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:9c681cefe72e257c6d58f839bb504f50bf259a0221c883fcc220f0755563fa46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:7e244fae615587335176db07e88b43eee5e4762f35306e17c13c68125d93b9bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124241217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76a4b2ed1b4014a9d638e15cd852544d8171c64ed78096fbe6e5a108fbf20b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:10:52 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 02:10:53 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 02:10:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:11:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:11:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:11:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:11:29 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:11:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f7bd4f1dda333860d0a1f30b5b8ec7ccedc7ea29bd90ba2b4cbc140f33c917`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5fa137d06e3953eab13f7fef4842cd2dcc883e398734c3ea923e9cc07a9ba`  
		Last Modified: Sat, 03 Apr 2021 02:13:37 GMT  
		Size: 87.6 MB (87576029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689a8c518900165fdb845e49162bbf561a2b291c79d6a7894e708a346c89ad74`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d4472cbcdcf08008f6be1e9d9a6e29f45aaead4cd0b4a6f4d0f7fb2892c9405
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121829873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43019a6fb0a9efab56424e9ce622b3aef9bf8505a4d51c7224f693a13d28a35d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:16:44 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:16:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:16:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:17:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:17:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:17:29 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:17:31 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:17:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e54de3da7dca0d12e5ba0bd3d6c00ed5f108cb341616aad40d750573525df`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72028e2877e63ed0d1ce1715663f908df19ca9beccce8e73c99e562d8a407b68`  
		Last Modified: Sat, 03 Apr 2021 06:20:47 GMT  
		Size: 86.7 MB (86653343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccaecdca9673211f0541464c67f03a0644842841e5cb8732d12ca0e804898b`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d2488fa0b439fae0630b2e7a8e757e8b6880afef3a20a004d39412f843655b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5a7472b0afafe37dbcff0a2e0db9ca30709f80d72bb941a056767f4e4d3f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:46:50 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:46:52 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:47:01 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:49:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:49:33 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:49:35 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:49:46 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:49:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a8ee527e9b195d270b34ff2ad5f33c81881e47c418b31a9dfd4fa359c72ec`  
		Last Modified: Sat, 03 Apr 2021 06:56:28 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3afa066a85db4a586c20e129f1dfdc7628d02e8f4d20a686e1d6a09f6fbae77`  
		Last Modified: Sat, 03 Apr 2021 06:56:49 GMT  
		Size: 92.2 MB (92198189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35002fcf886609f778e9c9844a7d94cc3a599a788b71339781f76f743df3fcba`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:9c681cefe72e257c6d58f839bb504f50bf259a0221c883fcc220f0755563fa46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7e244fae615587335176db07e88b43eee5e4762f35306e17c13c68125d93b9bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124241217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76a4b2ed1b4014a9d638e15cd852544d8171c64ed78096fbe6e5a108fbf20b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:10:52 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 02:10:53 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 02:10:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:11:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:11:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:11:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:11:29 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:11:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f7bd4f1dda333860d0a1f30b5b8ec7ccedc7ea29bd90ba2b4cbc140f33c917`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5fa137d06e3953eab13f7fef4842cd2dcc883e398734c3ea923e9cc07a9ba`  
		Last Modified: Sat, 03 Apr 2021 02:13:37 GMT  
		Size: 87.6 MB (87576029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689a8c518900165fdb845e49162bbf561a2b291c79d6a7894e708a346c89ad74`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d4472cbcdcf08008f6be1e9d9a6e29f45aaead4cd0b4a6f4d0f7fb2892c9405
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121829873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43019a6fb0a9efab56424e9ce622b3aef9bf8505a4d51c7224f693a13d28a35d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:16:44 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:16:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:16:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:17:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:17:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:17:29 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:17:31 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:17:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e54de3da7dca0d12e5ba0bd3d6c00ed5f108cb341616aad40d750573525df`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72028e2877e63ed0d1ce1715663f908df19ca9beccce8e73c99e562d8a407b68`  
		Last Modified: Sat, 03 Apr 2021 06:20:47 GMT  
		Size: 86.7 MB (86653343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccaecdca9673211f0541464c67f03a0644842841e5cb8732d12ca0e804898b`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d2488fa0b439fae0630b2e7a8e757e8b6880afef3a20a004d39412f843655b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5a7472b0afafe37dbcff0a2e0db9ca30709f80d72bb941a056767f4e4d3f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:46:50 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:46:52 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:47:01 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:49:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:49:33 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:49:35 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:49:46 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:49:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a8ee527e9b195d270b34ff2ad5f33c81881e47c418b31a9dfd4fa359c72ec`  
		Last Modified: Sat, 03 Apr 2021 06:56:28 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3afa066a85db4a586c20e129f1dfdc7628d02e8f4d20a686e1d6a09f6fbae77`  
		Last Modified: Sat, 03 Apr 2021 06:56:49 GMT  
		Size: 92.2 MB (92198189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35002fcf886609f778e9c9844a7d94cc3a599a788b71339781f76f743df3fcba`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1`

```console
$ docker pull mariadb@sha256:7d8cd037082bec716e981d013f4af35a9e63d3911d4118e59e624bcb4de9cb93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1` - linux; amd64

```console
$ docker pull mariadb@sha256:68865942c786f8be3a5e0f9604befe973bca071934b0d50fcf5054e337fa026d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113182165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25966872130ce8f9680a19b25df0c1ff869e9f1e837263c236e3ae79a67b1de3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:52:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 11:52:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:52:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 11:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 11:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:53:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 11:53:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 11:54:29 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 11:54:29 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 11:54:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 11:55:19 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 11:55:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 11:55:20 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:55:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:55:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:55:22 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 11:55:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f45e3863066b787d78c4ec01b2c4e92f6d137ef4437c29e5e73bed988dfad`  
		Last Modified: Fri, 26 Mar 2021 11:58:09 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02067a8ae4d84924bc19cbfde579f9713406eb19c0d3f87c45986b8895b2714c`  
		Last Modified: Fri, 26 Mar 2021 11:58:08 GMT  
		Size: 4.8 MB (4812807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7473d439bc3664901f88139c6861a1e4956bcf1cf70d786bc82d4ba1cdaed2`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 1.3 MB (1326645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cf83317dcdddfe432c60f9d2cf1f771499ba40e22b33bfbbb84d20805fdbad`  
		Last Modified: Fri, 26 Mar 2021 11:58:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee69a83317a136ef536a3deba8e13698b96dbcf4c6012e0684e6277dc495223d`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 932.4 KB (932437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794113981a4c21a389b894d6f7a52f01e0f0d813d017c61bd91e3e4bd4345620`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f41ac2b01acc892ff46826bd061adf320364ddde0cb5262c144fece2f999f57`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952aae72b155d6b192c33c0419a629bdd581862f2d3f238482fd64961a7ba70c`  
		Last Modified: Fri, 26 Mar 2021 11:58:58 GMT  
		Size: 79.4 MB (79385782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb6dc653a6f771362d60adf62bfb8fbc2f21026eadfee5b37b98eb024fed519`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47094fc27e45c46dc1990833b4a7a98597870760619db18cac915f3a681c517`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:65b9c55c60413541ce8e9312cdd03e201b3a84c747a310a8a976b97f9918adc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105803854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45b6cac51b70877410262d975ae791afa7b6186d767ce2caaab59180485fa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:17:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 14:17:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:00 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:18:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:39 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 14:18:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:20:12 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 14:20:13 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 14:20:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 14:21:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 14:21:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 14:21:16 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 14:21:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:21:19 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 14:21:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0531f1390e72fa0458c10d1ba9d70291a68a00c704cb777bc8761be2410925ff`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72819a073b5b56ccfeca252e766511185478741b4305af5c57136bf9ad22022a`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 4.4 MB (4395449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca3c34ec85cf0e786eef18f3472109ebdcc4c3fe0bdc1d98375ee9717fd1c9f`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 1.3 MB (1263787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c024f04ce1ac2812c515c15e819057471ab1c1e93a6fab65ebe924abe9892c`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d05c8a0a6ab565b8b1686dda41f172ecd8a51fa391fcaea711d14d2e7a87fc`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 925.4 KB (925365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8e152c889b8e6ed5cab4ac0b79280a47d4fd0b8f6f88a40f9d55f779a5973`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0ba9d2f1255fc498035f8d64e43cf8a4b03cb3fdd7cf1a6aa14f785b49b8f3`  
		Last Modified: Fri, 26 Mar 2021 14:24:36 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b0175a2aa118308b29a712a8375c2d14e84c8d4c16c41a489874f8b9a2bdc4`  
		Last Modified: Fri, 26 Mar 2021 14:24:53 GMT  
		Size: 75.5 MB (75472751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acee8a94308f3135d948032bad1fa4698ad905afc6f3f19c7fb42cb8a5be53a`  
		Last Modified: Fri, 26 Mar 2021 14:24:37 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a15515206c825a4e0d4616357485dd549d6185cca88048d844d88e5468375dd`  
		Last Modified: Fri, 26 Mar 2021 14:24:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3019606aa8dce9fb2ed58bca649fb73d9e3db51296fe0e286563e2cbd2884b3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd1b5f84cf762ec441cffe9055a6500dee1d7525605ab4215c5eb269a215b96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 16:30:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 16:32:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:32:39 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 16:33:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 16:34:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 16:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 16:34:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 16:39:45 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 16:39:50 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 16:39:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 16:43:59 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 16:44:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 16:44:14 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:44:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:44:30 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 16:44:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855e1295dc26a0c9b74e4482407b555044126c274cf25d14a488b5ac4cb2bc2`  
		Last Modified: Fri, 26 Mar 2021 16:47:30 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abddac719dc870aff20cad4f746209f976a1313fc6cd4f59f48df1e5584cf9`  
		Last Modified: Fri, 26 Mar 2021 16:47:32 GMT  
		Size: 5.6 MB (5630341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d763841542bc8c30fad86aca6afadc38ca331054204137f760297438be1e067`  
		Last Modified: Fri, 26 Mar 2021 16:47:31 GMT  
		Size: 1.2 MB (1246971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6807c27a6f6e0149bb26f56402a780b429982e4c3f8094b552ac3754c49a832`  
		Last Modified: Fri, 26 Mar 2021 16:47:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427969943d1691cb07a5bf70b1643649abc5bc2f42d5caf89f78f72f9a52d94`  
		Last Modified: Fri, 26 Mar 2021 16:47:27 GMT  
		Size: 934.9 KB (934923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240458af14f0c26fc73c4df8188481166204069bcdb39c5cb497fb5b98992280`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad938147d1ca1cbc6618479839fd25f1ee383452401205bf6f8107940572b04`  
		Last Modified: Fri, 26 Mar 2021 16:47:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b0614642d411a24925c200821fcbf5cc36003c28fbb4a2ccfb6d2eab44a6ee`  
		Last Modified: Fri, 26 Mar 2021 16:48:15 GMT  
		Size: 79.9 MB (79923559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fddb071b1218c89b078d27b9d27b485fdf42c41933bf31b1dbac0695de608b`  
		Last Modified: Fri, 26 Mar 2021 16:47:58 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f31dd5c0d1a0af286f8b898b2c08428db852c7db39b2974d039b68d46952f5`  
		Last Modified: Fri, 26 Mar 2021 16:47:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1-bionic`

```console
$ docker pull mariadb@sha256:7d8cd037082bec716e981d013f4af35a9e63d3911d4118e59e624bcb4de9cb93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:68865942c786f8be3a5e0f9604befe973bca071934b0d50fcf5054e337fa026d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113182165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25966872130ce8f9680a19b25df0c1ff869e9f1e837263c236e3ae79a67b1de3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:52:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 11:52:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:52:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 11:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 11:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:53:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 11:53:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 11:54:29 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 11:54:29 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 11:54:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 11:55:19 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 11:55:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 11:55:20 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:55:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:55:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:55:22 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 11:55:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f45e3863066b787d78c4ec01b2c4e92f6d137ef4437c29e5e73bed988dfad`  
		Last Modified: Fri, 26 Mar 2021 11:58:09 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02067a8ae4d84924bc19cbfde579f9713406eb19c0d3f87c45986b8895b2714c`  
		Last Modified: Fri, 26 Mar 2021 11:58:08 GMT  
		Size: 4.8 MB (4812807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7473d439bc3664901f88139c6861a1e4956bcf1cf70d786bc82d4ba1cdaed2`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 1.3 MB (1326645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cf83317dcdddfe432c60f9d2cf1f771499ba40e22b33bfbbb84d20805fdbad`  
		Last Modified: Fri, 26 Mar 2021 11:58:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee69a83317a136ef536a3deba8e13698b96dbcf4c6012e0684e6277dc495223d`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 932.4 KB (932437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794113981a4c21a389b894d6f7a52f01e0f0d813d017c61bd91e3e4bd4345620`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f41ac2b01acc892ff46826bd061adf320364ddde0cb5262c144fece2f999f57`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952aae72b155d6b192c33c0419a629bdd581862f2d3f238482fd64961a7ba70c`  
		Last Modified: Fri, 26 Mar 2021 11:58:58 GMT  
		Size: 79.4 MB (79385782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb6dc653a6f771362d60adf62bfb8fbc2f21026eadfee5b37b98eb024fed519`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47094fc27e45c46dc1990833b4a7a98597870760619db18cac915f3a681c517`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:65b9c55c60413541ce8e9312cdd03e201b3a84c747a310a8a976b97f9918adc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105803854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45b6cac51b70877410262d975ae791afa7b6186d767ce2caaab59180485fa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:17:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 14:17:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:00 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:18:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:39 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 14:18:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:20:12 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 14:20:13 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 14:20:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 14:21:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 14:21:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 14:21:16 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 14:21:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:21:19 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 14:21:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0531f1390e72fa0458c10d1ba9d70291a68a00c704cb777bc8761be2410925ff`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72819a073b5b56ccfeca252e766511185478741b4305af5c57136bf9ad22022a`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 4.4 MB (4395449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca3c34ec85cf0e786eef18f3472109ebdcc4c3fe0bdc1d98375ee9717fd1c9f`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 1.3 MB (1263787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c024f04ce1ac2812c515c15e819057471ab1c1e93a6fab65ebe924abe9892c`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d05c8a0a6ab565b8b1686dda41f172ecd8a51fa391fcaea711d14d2e7a87fc`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 925.4 KB (925365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8e152c889b8e6ed5cab4ac0b79280a47d4fd0b8f6f88a40f9d55f779a5973`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0ba9d2f1255fc498035f8d64e43cf8a4b03cb3fdd7cf1a6aa14f785b49b8f3`  
		Last Modified: Fri, 26 Mar 2021 14:24:36 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b0175a2aa118308b29a712a8375c2d14e84c8d4c16c41a489874f8b9a2bdc4`  
		Last Modified: Fri, 26 Mar 2021 14:24:53 GMT  
		Size: 75.5 MB (75472751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acee8a94308f3135d948032bad1fa4698ad905afc6f3f19c7fb42cb8a5be53a`  
		Last Modified: Fri, 26 Mar 2021 14:24:37 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a15515206c825a4e0d4616357485dd549d6185cca88048d844d88e5468375dd`  
		Last Modified: Fri, 26 Mar 2021 14:24:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3019606aa8dce9fb2ed58bca649fb73d9e3db51296fe0e286563e2cbd2884b3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd1b5f84cf762ec441cffe9055a6500dee1d7525605ab4215c5eb269a215b96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 16:30:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 16:32:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:32:39 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 16:33:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 16:34:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 16:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 16:34:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 16:39:45 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 16:39:50 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 16:39:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 16:43:59 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 16:44:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 16:44:14 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:44:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:44:30 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 16:44:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855e1295dc26a0c9b74e4482407b555044126c274cf25d14a488b5ac4cb2bc2`  
		Last Modified: Fri, 26 Mar 2021 16:47:30 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abddac719dc870aff20cad4f746209f976a1313fc6cd4f59f48df1e5584cf9`  
		Last Modified: Fri, 26 Mar 2021 16:47:32 GMT  
		Size: 5.6 MB (5630341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d763841542bc8c30fad86aca6afadc38ca331054204137f760297438be1e067`  
		Last Modified: Fri, 26 Mar 2021 16:47:31 GMT  
		Size: 1.2 MB (1246971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6807c27a6f6e0149bb26f56402a780b429982e4c3f8094b552ac3754c49a832`  
		Last Modified: Fri, 26 Mar 2021 16:47:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427969943d1691cb07a5bf70b1643649abc5bc2f42d5caf89f78f72f9a52d94`  
		Last Modified: Fri, 26 Mar 2021 16:47:27 GMT  
		Size: 934.9 KB (934923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240458af14f0c26fc73c4df8188481166204069bcdb39c5cb497fb5b98992280`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad938147d1ca1cbc6618479839fd25f1ee383452401205bf6f8107940572b04`  
		Last Modified: Fri, 26 Mar 2021 16:47:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b0614642d411a24925c200821fcbf5cc36003c28fbb4a2ccfb6d2eab44a6ee`  
		Last Modified: Fri, 26 Mar 2021 16:48:15 GMT  
		Size: 79.9 MB (79923559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fddb071b1218c89b078d27b9d27b485fdf42c41933bf31b1dbac0695de608b`  
		Last Modified: Fri, 26 Mar 2021 16:47:58 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f31dd5c0d1a0af286f8b898b2c08428db852c7db39b2974d039b68d46952f5`  
		Last Modified: Fri, 26 Mar 2021 16:47:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48`

```console
$ docker pull mariadb@sha256:7d8cd037082bec716e981d013f4af35a9e63d3911d4118e59e624bcb4de9cb93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48` - linux; amd64

```console
$ docker pull mariadb@sha256:68865942c786f8be3a5e0f9604befe973bca071934b0d50fcf5054e337fa026d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113182165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25966872130ce8f9680a19b25df0c1ff869e9f1e837263c236e3ae79a67b1de3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:52:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 11:52:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:52:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 11:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 11:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:53:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 11:53:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 11:54:29 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 11:54:29 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 11:54:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 11:55:19 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 11:55:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 11:55:20 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:55:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:55:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:55:22 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 11:55:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f45e3863066b787d78c4ec01b2c4e92f6d137ef4437c29e5e73bed988dfad`  
		Last Modified: Fri, 26 Mar 2021 11:58:09 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02067a8ae4d84924bc19cbfde579f9713406eb19c0d3f87c45986b8895b2714c`  
		Last Modified: Fri, 26 Mar 2021 11:58:08 GMT  
		Size: 4.8 MB (4812807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7473d439bc3664901f88139c6861a1e4956bcf1cf70d786bc82d4ba1cdaed2`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 1.3 MB (1326645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cf83317dcdddfe432c60f9d2cf1f771499ba40e22b33bfbbb84d20805fdbad`  
		Last Modified: Fri, 26 Mar 2021 11:58:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee69a83317a136ef536a3deba8e13698b96dbcf4c6012e0684e6277dc495223d`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 932.4 KB (932437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794113981a4c21a389b894d6f7a52f01e0f0d813d017c61bd91e3e4bd4345620`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f41ac2b01acc892ff46826bd061adf320364ddde0cb5262c144fece2f999f57`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952aae72b155d6b192c33c0419a629bdd581862f2d3f238482fd64961a7ba70c`  
		Last Modified: Fri, 26 Mar 2021 11:58:58 GMT  
		Size: 79.4 MB (79385782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb6dc653a6f771362d60adf62bfb8fbc2f21026eadfee5b37b98eb024fed519`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47094fc27e45c46dc1990833b4a7a98597870760619db18cac915f3a681c517`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:65b9c55c60413541ce8e9312cdd03e201b3a84c747a310a8a976b97f9918adc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105803854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45b6cac51b70877410262d975ae791afa7b6186d767ce2caaab59180485fa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:17:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 14:17:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:00 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:18:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:39 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 14:18:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:20:12 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 14:20:13 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 14:20:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 14:21:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 14:21:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 14:21:16 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 14:21:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:21:19 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 14:21:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0531f1390e72fa0458c10d1ba9d70291a68a00c704cb777bc8761be2410925ff`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72819a073b5b56ccfeca252e766511185478741b4305af5c57136bf9ad22022a`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 4.4 MB (4395449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca3c34ec85cf0e786eef18f3472109ebdcc4c3fe0bdc1d98375ee9717fd1c9f`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 1.3 MB (1263787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c024f04ce1ac2812c515c15e819057471ab1c1e93a6fab65ebe924abe9892c`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d05c8a0a6ab565b8b1686dda41f172ecd8a51fa391fcaea711d14d2e7a87fc`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 925.4 KB (925365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8e152c889b8e6ed5cab4ac0b79280a47d4fd0b8f6f88a40f9d55f779a5973`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0ba9d2f1255fc498035f8d64e43cf8a4b03cb3fdd7cf1a6aa14f785b49b8f3`  
		Last Modified: Fri, 26 Mar 2021 14:24:36 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b0175a2aa118308b29a712a8375c2d14e84c8d4c16c41a489874f8b9a2bdc4`  
		Last Modified: Fri, 26 Mar 2021 14:24:53 GMT  
		Size: 75.5 MB (75472751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acee8a94308f3135d948032bad1fa4698ad905afc6f3f19c7fb42cb8a5be53a`  
		Last Modified: Fri, 26 Mar 2021 14:24:37 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a15515206c825a4e0d4616357485dd549d6185cca88048d844d88e5468375dd`  
		Last Modified: Fri, 26 Mar 2021 14:24:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3019606aa8dce9fb2ed58bca649fb73d9e3db51296fe0e286563e2cbd2884b3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd1b5f84cf762ec441cffe9055a6500dee1d7525605ab4215c5eb269a215b96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 16:30:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 16:32:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:32:39 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 16:33:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 16:34:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 16:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 16:34:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 16:39:45 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 16:39:50 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 16:39:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 16:43:59 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 16:44:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 16:44:14 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:44:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:44:30 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 16:44:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855e1295dc26a0c9b74e4482407b555044126c274cf25d14a488b5ac4cb2bc2`  
		Last Modified: Fri, 26 Mar 2021 16:47:30 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abddac719dc870aff20cad4f746209f976a1313fc6cd4f59f48df1e5584cf9`  
		Last Modified: Fri, 26 Mar 2021 16:47:32 GMT  
		Size: 5.6 MB (5630341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d763841542bc8c30fad86aca6afadc38ca331054204137f760297438be1e067`  
		Last Modified: Fri, 26 Mar 2021 16:47:31 GMT  
		Size: 1.2 MB (1246971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6807c27a6f6e0149bb26f56402a780b429982e4c3f8094b552ac3754c49a832`  
		Last Modified: Fri, 26 Mar 2021 16:47:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427969943d1691cb07a5bf70b1643649abc5bc2f42d5caf89f78f72f9a52d94`  
		Last Modified: Fri, 26 Mar 2021 16:47:27 GMT  
		Size: 934.9 KB (934923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240458af14f0c26fc73c4df8188481166204069bcdb39c5cb497fb5b98992280`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad938147d1ca1cbc6618479839fd25f1ee383452401205bf6f8107940572b04`  
		Last Modified: Fri, 26 Mar 2021 16:47:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b0614642d411a24925c200821fcbf5cc36003c28fbb4a2ccfb6d2eab44a6ee`  
		Last Modified: Fri, 26 Mar 2021 16:48:15 GMT  
		Size: 79.9 MB (79923559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fddb071b1218c89b078d27b9d27b485fdf42c41933bf31b1dbac0695de608b`  
		Last Modified: Fri, 26 Mar 2021 16:47:58 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f31dd5c0d1a0af286f8b898b2c08428db852c7db39b2974d039b68d46952f5`  
		Last Modified: Fri, 26 Mar 2021 16:47:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48-bionic`

```console
$ docker pull mariadb@sha256:7d8cd037082bec716e981d013f4af35a9e63d3911d4118e59e624bcb4de9cb93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:68865942c786f8be3a5e0f9604befe973bca071934b0d50fcf5054e337fa026d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113182165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25966872130ce8f9680a19b25df0c1ff869e9f1e837263c236e3ae79a67b1de3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:52:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 11:52:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:52:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 11:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 11:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:53:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 11:53:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 11:54:29 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 11:54:29 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 11:54:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 11:55:19 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 11:55:20 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 11:55:20 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:55:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:55:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:55:22 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 11:55:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f45e3863066b787d78c4ec01b2c4e92f6d137ef4437c29e5e73bed988dfad`  
		Last Modified: Fri, 26 Mar 2021 11:58:09 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02067a8ae4d84924bc19cbfde579f9713406eb19c0d3f87c45986b8895b2714c`  
		Last Modified: Fri, 26 Mar 2021 11:58:08 GMT  
		Size: 4.8 MB (4812807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7473d439bc3664901f88139c6861a1e4956bcf1cf70d786bc82d4ba1cdaed2`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 1.3 MB (1326645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cf83317dcdddfe432c60f9d2cf1f771499ba40e22b33bfbbb84d20805fdbad`  
		Last Modified: Fri, 26 Mar 2021 11:58:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee69a83317a136ef536a3deba8e13698b96dbcf4c6012e0684e6277dc495223d`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 932.4 KB (932437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794113981a4c21a389b894d6f7a52f01e0f0d813d017c61bd91e3e4bd4345620`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f41ac2b01acc892ff46826bd061adf320364ddde0cb5262c144fece2f999f57`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952aae72b155d6b192c33c0419a629bdd581862f2d3f238482fd64961a7ba70c`  
		Last Modified: Fri, 26 Mar 2021 11:58:58 GMT  
		Size: 79.4 MB (79385782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb6dc653a6f771362d60adf62bfb8fbc2f21026eadfee5b37b98eb024fed519`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47094fc27e45c46dc1990833b4a7a98597870760619db18cac915f3a681c517`  
		Last Modified: Fri, 26 Mar 2021 11:58:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:65b9c55c60413541ce8e9312cdd03e201b3a84c747a310a8a976b97f9918adc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105803854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45b6cac51b70877410262d975ae791afa7b6186d767ce2caaab59180485fa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:17:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 14:17:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:00 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:18:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:39 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 14:18:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:20:12 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 14:20:13 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 14:20:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 14:21:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 14:21:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 14:21:16 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:21:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 14:21:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:21:19 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 14:21:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0531f1390e72fa0458c10d1ba9d70291a68a00c704cb777bc8761be2410925ff`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72819a073b5b56ccfeca252e766511185478741b4305af5c57136bf9ad22022a`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 4.4 MB (4395449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca3c34ec85cf0e786eef18f3472109ebdcc4c3fe0bdc1d98375ee9717fd1c9f`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 1.3 MB (1263787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c024f04ce1ac2812c515c15e819057471ab1c1e93a6fab65ebe924abe9892c`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d05c8a0a6ab565b8b1686dda41f172ecd8a51fa391fcaea711d14d2e7a87fc`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 925.4 KB (925365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8e152c889b8e6ed5cab4ac0b79280a47d4fd0b8f6f88a40f9d55f779a5973`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0ba9d2f1255fc498035f8d64e43cf8a4b03cb3fdd7cf1a6aa14f785b49b8f3`  
		Last Modified: Fri, 26 Mar 2021 14:24:36 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b0175a2aa118308b29a712a8375c2d14e84c8d4c16c41a489874f8b9a2bdc4`  
		Last Modified: Fri, 26 Mar 2021 14:24:53 GMT  
		Size: 75.5 MB (75472751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acee8a94308f3135d948032bad1fa4698ad905afc6f3f19c7fb42cb8a5be53a`  
		Last Modified: Fri, 26 Mar 2021 14:24:37 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a15515206c825a4e0d4616357485dd549d6185cca88048d844d88e5468375dd`  
		Last Modified: Fri, 26 Mar 2021 14:24:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3019606aa8dce9fb2ed58bca649fb73d9e3db51296fe0e286563e2cbd2884b3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd1b5f84cf762ec441cffe9055a6500dee1d7525605ab4215c5eb269a215b96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 16:30:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 16:32:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:32:39 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 16:33:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 16:34:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 16:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 16:34:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 16:39:45 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 26 Mar 2021 16:39:50 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 26 Mar 2021 16:39:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 16:43:59 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 16:44:11 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 16:44:14 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:44:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 16:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:44:30 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 16:44:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855e1295dc26a0c9b74e4482407b555044126c274cf25d14a488b5ac4cb2bc2`  
		Last Modified: Fri, 26 Mar 2021 16:47:30 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abddac719dc870aff20cad4f746209f976a1313fc6cd4f59f48df1e5584cf9`  
		Last Modified: Fri, 26 Mar 2021 16:47:32 GMT  
		Size: 5.6 MB (5630341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d763841542bc8c30fad86aca6afadc38ca331054204137f760297438be1e067`  
		Last Modified: Fri, 26 Mar 2021 16:47:31 GMT  
		Size: 1.2 MB (1246971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6807c27a6f6e0149bb26f56402a780b429982e4c3f8094b552ac3754c49a832`  
		Last Modified: Fri, 26 Mar 2021 16:47:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427969943d1691cb07a5bf70b1643649abc5bc2f42d5caf89f78f72f9a52d94`  
		Last Modified: Fri, 26 Mar 2021 16:47:27 GMT  
		Size: 934.9 KB (934923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240458af14f0c26fc73c4df8188481166204069bcdb39c5cb497fb5b98992280`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad938147d1ca1cbc6618479839fd25f1ee383452401205bf6f8107940572b04`  
		Last Modified: Fri, 26 Mar 2021 16:47:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b0614642d411a24925c200821fcbf5cc36003c28fbb4a2ccfb6d2eab44a6ee`  
		Last Modified: Fri, 26 Mar 2021 16:48:15 GMT  
		Size: 79.9 MB (79923559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fddb071b1218c89b078d27b9d27b485fdf42c41933bf31b1dbac0695de608b`  
		Last Modified: Fri, 26 Mar 2021 16:47:58 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f31dd5c0d1a0af286f8b898b2c08428db852c7db39b2974d039b68d46952f5`  
		Last Modified: Fri, 26 Mar 2021 16:47:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:087f643fad1d66e868a27018e033ede151020ce2e327ddc988e49d6ee22db9b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:f70fbb0afeafb3a04d51650605ace81fa236c27fafa48b41b76d2c6485431359
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107995675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d6a130fc1fe1f83cfa7e55ab0165ad0f8f52d7c3900385ab75339bc6def686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:52:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 11:52:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:52:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 11:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 11:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:53:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 11:53:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 11:53:32 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 11:53:32 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 11:53:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 11:54:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 11:54:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 11:54:21 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:54:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:54:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:54:23 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 11:54:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f45e3863066b787d78c4ec01b2c4e92f6d137ef4437c29e5e73bed988dfad`  
		Last Modified: Fri, 26 Mar 2021 11:58:09 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02067a8ae4d84924bc19cbfde579f9713406eb19c0d3f87c45986b8895b2714c`  
		Last Modified: Fri, 26 Mar 2021 11:58:08 GMT  
		Size: 4.8 MB (4812807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7473d439bc3664901f88139c6861a1e4956bcf1cf70d786bc82d4ba1cdaed2`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 1.3 MB (1326645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cf83317dcdddfe432c60f9d2cf1f771499ba40e22b33bfbbb84d20805fdbad`  
		Last Modified: Fri, 26 Mar 2021 11:58:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee69a83317a136ef536a3deba8e13698b96dbcf4c6012e0684e6277dc495223d`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 932.4 KB (932437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794113981a4c21a389b894d6f7a52f01e0f0d813d017c61bd91e3e4bd4345620`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab47c6c83bc366ae30f4ad6e5ab8e0ceacf42f683d7d85d7e08527cf5518e07e`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206171cc1dd1d1ad0c19e8554e05f49409a4f50b6d7d12184343850960c2bb32`  
		Last Modified: Fri, 26 Mar 2021 11:58:21 GMT  
		Size: 74.2 MB (74199294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b18a9d2c285b7cff0a91f215beaa5587cad9ea79b10bc7db67771f46be621d`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e643e5ef37013d5efddc6e3d860f218c6c214d25a267116c0a015579af46c2a`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0eefbab6ec39ca851d787312bbfcaeac7e292708dbabadb3d8164b33f7d251e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103143249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:393378e6c691ca88bd380e1007ad74bac5c360876fa925ae0a719c0661fac6e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:17:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 14:17:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:00 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:18:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:39 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 14:18:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:18:43 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 14:18:44 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 14:18:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 14:19:42 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 14:19:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 14:19:47 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:19:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 14:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:19:52 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 14:19:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0531f1390e72fa0458c10d1ba9d70291a68a00c704cb777bc8761be2410925ff`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72819a073b5b56ccfeca252e766511185478741b4305af5c57136bf9ad22022a`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 4.4 MB (4395449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca3c34ec85cf0e786eef18f3472109ebdcc4c3fe0bdc1d98375ee9717fd1c9f`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 1.3 MB (1263787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c024f04ce1ac2812c515c15e819057471ab1c1e93a6fab65ebe924abe9892c`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d05c8a0a6ab565b8b1686dda41f172ecd8a51fa391fcaea711d14d2e7a87fc`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 925.4 KB (925365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8e152c889b8e6ed5cab4ac0b79280a47d4fd0b8f6f88a40f9d55f779a5973`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56594ae78dce4d478095518713b80e59c2eaf613b0df64f5c6c4f5e513ddca30`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6834e4c7d6cfaeed1aa24a41cebcc7fa5ef6ace81ce67476fd0a327cf1550c4`  
		Last Modified: Fri, 26 Mar 2021 14:24:23 GMT  
		Size: 72.8 MB (72812142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9a00e9a2f9c7edf717bd86fbe2c28f85388e702cbfcfbc5a3a75e089b7d367`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54c240903607e7bfceb958126e8c5cd48214de9e97b4d67528d4e108f6b613e`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:86839d9106cbab2f4ee05188ba1c4240b825978621fa3427a97df903410bd759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116018747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5737a561d5c314f5bc83542d0b66f608b8e1380bf6b45269072764e566a14f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 16:30:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 16:32:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:32:39 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 16:33:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 16:34:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 16:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 16:34:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 16:34:47 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 16:34:52 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 16:35:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 16:38:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 16:38:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 16:38:57 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:39:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 16:39:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:39:17 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 16:39:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855e1295dc26a0c9b74e4482407b555044126c274cf25d14a488b5ac4cb2bc2`  
		Last Modified: Fri, 26 Mar 2021 16:47:30 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abddac719dc870aff20cad4f746209f976a1313fc6cd4f59f48df1e5584cf9`  
		Last Modified: Fri, 26 Mar 2021 16:47:32 GMT  
		Size: 5.6 MB (5630341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d763841542bc8c30fad86aca6afadc38ca331054204137f760297438be1e067`  
		Last Modified: Fri, 26 Mar 2021 16:47:31 GMT  
		Size: 1.2 MB (1246971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6807c27a6f6e0149bb26f56402a780b429982e4c3f8094b552ac3754c49a832`  
		Last Modified: Fri, 26 Mar 2021 16:47:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427969943d1691cb07a5bf70b1643649abc5bc2f42d5caf89f78f72f9a52d94`  
		Last Modified: Fri, 26 Mar 2021 16:47:27 GMT  
		Size: 934.9 KB (934923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240458af14f0c26fc73c4df8188481166204069bcdb39c5cb497fb5b98992280`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be7dd9df0131fba73b62e4a14056357bcb7eff9ee05e08a6b5a45ca8cb06a3`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8796b8c85e511e6d96632891801fc8335b04888982374bc30b96b31bec375496`  
		Last Modified: Fri, 26 Mar 2021 16:47:41 GMT  
		Size: 77.8 MB (77769530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc538d9d2381f73dd75c49b34017a1f2ccf08b96ba7aaaee50b2645d821985c`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312d5019b3781430c4e0ce58958ec15a58cee9035d9cd429dcc9e7960c9c9fa7`  
		Last Modified: Fri, 26 Mar 2021 16:47:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:087f643fad1d66e868a27018e033ede151020ce2e327ddc988e49d6ee22db9b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:f70fbb0afeafb3a04d51650605ace81fa236c27fafa48b41b76d2c6485431359
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107995675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d6a130fc1fe1f83cfa7e55ab0165ad0f8f52d7c3900385ab75339bc6def686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:52:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 11:52:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:52:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 11:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 11:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:53:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 11:53:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 11:53:32 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 11:53:32 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 11:53:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 11:54:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 11:54:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 11:54:21 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:54:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:54:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:54:23 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 11:54:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f45e3863066b787d78c4ec01b2c4e92f6d137ef4437c29e5e73bed988dfad`  
		Last Modified: Fri, 26 Mar 2021 11:58:09 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02067a8ae4d84924bc19cbfde579f9713406eb19c0d3f87c45986b8895b2714c`  
		Last Modified: Fri, 26 Mar 2021 11:58:08 GMT  
		Size: 4.8 MB (4812807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7473d439bc3664901f88139c6861a1e4956bcf1cf70d786bc82d4ba1cdaed2`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 1.3 MB (1326645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cf83317dcdddfe432c60f9d2cf1f771499ba40e22b33bfbbb84d20805fdbad`  
		Last Modified: Fri, 26 Mar 2021 11:58:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee69a83317a136ef536a3deba8e13698b96dbcf4c6012e0684e6277dc495223d`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 932.4 KB (932437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794113981a4c21a389b894d6f7a52f01e0f0d813d017c61bd91e3e4bd4345620`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab47c6c83bc366ae30f4ad6e5ab8e0ceacf42f683d7d85d7e08527cf5518e07e`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206171cc1dd1d1ad0c19e8554e05f49409a4f50b6d7d12184343850960c2bb32`  
		Last Modified: Fri, 26 Mar 2021 11:58:21 GMT  
		Size: 74.2 MB (74199294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b18a9d2c285b7cff0a91f215beaa5587cad9ea79b10bc7db67771f46be621d`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e643e5ef37013d5efddc6e3d860f218c6c214d25a267116c0a015579af46c2a`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0eefbab6ec39ca851d787312bbfcaeac7e292708dbabadb3d8164b33f7d251e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103143249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:393378e6c691ca88bd380e1007ad74bac5c360876fa925ae0a719c0661fac6e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:17:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 14:17:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:00 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:18:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:39 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 14:18:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:18:43 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 14:18:44 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 14:18:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 14:19:42 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 14:19:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 14:19:47 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:19:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 14:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:19:52 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 14:19:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0531f1390e72fa0458c10d1ba9d70291a68a00c704cb777bc8761be2410925ff`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72819a073b5b56ccfeca252e766511185478741b4305af5c57136bf9ad22022a`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 4.4 MB (4395449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca3c34ec85cf0e786eef18f3472109ebdcc4c3fe0bdc1d98375ee9717fd1c9f`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 1.3 MB (1263787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c024f04ce1ac2812c515c15e819057471ab1c1e93a6fab65ebe924abe9892c`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d05c8a0a6ab565b8b1686dda41f172ecd8a51fa391fcaea711d14d2e7a87fc`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 925.4 KB (925365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8e152c889b8e6ed5cab4ac0b79280a47d4fd0b8f6f88a40f9d55f779a5973`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56594ae78dce4d478095518713b80e59c2eaf613b0df64f5c6c4f5e513ddca30`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6834e4c7d6cfaeed1aa24a41cebcc7fa5ef6ace81ce67476fd0a327cf1550c4`  
		Last Modified: Fri, 26 Mar 2021 14:24:23 GMT  
		Size: 72.8 MB (72812142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9a00e9a2f9c7edf717bd86fbe2c28f85388e702cbfcfbc5a3a75e089b7d367`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54c240903607e7bfceb958126e8c5cd48214de9e97b4d67528d4e108f6b613e`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:86839d9106cbab2f4ee05188ba1c4240b825978621fa3427a97df903410bd759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116018747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5737a561d5c314f5bc83542d0b66f608b8e1380bf6b45269072764e566a14f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 16:30:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 16:32:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:32:39 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 16:33:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 16:34:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 16:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 16:34:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 16:34:47 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 16:34:52 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 16:35:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 16:38:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 16:38:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 16:38:57 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:39:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 16:39:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:39:17 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 16:39:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855e1295dc26a0c9b74e4482407b555044126c274cf25d14a488b5ac4cb2bc2`  
		Last Modified: Fri, 26 Mar 2021 16:47:30 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abddac719dc870aff20cad4f746209f976a1313fc6cd4f59f48df1e5584cf9`  
		Last Modified: Fri, 26 Mar 2021 16:47:32 GMT  
		Size: 5.6 MB (5630341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d763841542bc8c30fad86aca6afadc38ca331054204137f760297438be1e067`  
		Last Modified: Fri, 26 Mar 2021 16:47:31 GMT  
		Size: 1.2 MB (1246971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6807c27a6f6e0149bb26f56402a780b429982e4c3f8094b552ac3754c49a832`  
		Last Modified: Fri, 26 Mar 2021 16:47:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427969943d1691cb07a5bf70b1643649abc5bc2f42d5caf89f78f72f9a52d94`  
		Last Modified: Fri, 26 Mar 2021 16:47:27 GMT  
		Size: 934.9 KB (934923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240458af14f0c26fc73c4df8188481166204069bcdb39c5cb497fb5b98992280`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be7dd9df0131fba73b62e4a14056357bcb7eff9ee05e08a6b5a45ca8cb06a3`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8796b8c85e511e6d96632891801fc8335b04888982374bc30b96b31bec375496`  
		Last Modified: Fri, 26 Mar 2021 16:47:41 GMT  
		Size: 77.8 MB (77769530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc538d9d2381f73dd75c49b34017a1f2ccf08b96ba7aaaee50b2645d821985c`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312d5019b3781430c4e0ce58958ec15a58cee9035d9cd429dcc9e7960c9c9fa7`  
		Last Modified: Fri, 26 Mar 2021 16:47:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.37`

```console
$ docker pull mariadb@sha256:087f643fad1d66e868a27018e033ede151020ce2e327ddc988e49d6ee22db9b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.37` - linux; amd64

```console
$ docker pull mariadb@sha256:f70fbb0afeafb3a04d51650605ace81fa236c27fafa48b41b76d2c6485431359
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107995675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d6a130fc1fe1f83cfa7e55ab0165ad0f8f52d7c3900385ab75339bc6def686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:52:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 11:52:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:52:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 11:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 11:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:53:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 11:53:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 11:53:32 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 11:53:32 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 11:53:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 11:54:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 11:54:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 11:54:21 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:54:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:54:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:54:23 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 11:54:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f45e3863066b787d78c4ec01b2c4e92f6d137ef4437c29e5e73bed988dfad`  
		Last Modified: Fri, 26 Mar 2021 11:58:09 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02067a8ae4d84924bc19cbfde579f9713406eb19c0d3f87c45986b8895b2714c`  
		Last Modified: Fri, 26 Mar 2021 11:58:08 GMT  
		Size: 4.8 MB (4812807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7473d439bc3664901f88139c6861a1e4956bcf1cf70d786bc82d4ba1cdaed2`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 1.3 MB (1326645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cf83317dcdddfe432c60f9d2cf1f771499ba40e22b33bfbbb84d20805fdbad`  
		Last Modified: Fri, 26 Mar 2021 11:58:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee69a83317a136ef536a3deba8e13698b96dbcf4c6012e0684e6277dc495223d`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 932.4 KB (932437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794113981a4c21a389b894d6f7a52f01e0f0d813d017c61bd91e3e4bd4345620`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab47c6c83bc366ae30f4ad6e5ab8e0ceacf42f683d7d85d7e08527cf5518e07e`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206171cc1dd1d1ad0c19e8554e05f49409a4f50b6d7d12184343850960c2bb32`  
		Last Modified: Fri, 26 Mar 2021 11:58:21 GMT  
		Size: 74.2 MB (74199294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b18a9d2c285b7cff0a91f215beaa5587cad9ea79b10bc7db67771f46be621d`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e643e5ef37013d5efddc6e3d860f218c6c214d25a267116c0a015579af46c2a`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0eefbab6ec39ca851d787312bbfcaeac7e292708dbabadb3d8164b33f7d251e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103143249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:393378e6c691ca88bd380e1007ad74bac5c360876fa925ae0a719c0661fac6e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:17:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 14:17:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:00 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:18:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:39 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 14:18:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:18:43 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 14:18:44 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 14:18:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 14:19:42 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 14:19:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 14:19:47 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:19:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 14:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:19:52 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 14:19:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0531f1390e72fa0458c10d1ba9d70291a68a00c704cb777bc8761be2410925ff`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72819a073b5b56ccfeca252e766511185478741b4305af5c57136bf9ad22022a`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 4.4 MB (4395449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca3c34ec85cf0e786eef18f3472109ebdcc4c3fe0bdc1d98375ee9717fd1c9f`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 1.3 MB (1263787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c024f04ce1ac2812c515c15e819057471ab1c1e93a6fab65ebe924abe9892c`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d05c8a0a6ab565b8b1686dda41f172ecd8a51fa391fcaea711d14d2e7a87fc`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 925.4 KB (925365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8e152c889b8e6ed5cab4ac0b79280a47d4fd0b8f6f88a40f9d55f779a5973`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56594ae78dce4d478095518713b80e59c2eaf613b0df64f5c6c4f5e513ddca30`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6834e4c7d6cfaeed1aa24a41cebcc7fa5ef6ace81ce67476fd0a327cf1550c4`  
		Last Modified: Fri, 26 Mar 2021 14:24:23 GMT  
		Size: 72.8 MB (72812142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9a00e9a2f9c7edf717bd86fbe2c28f85388e702cbfcfbc5a3a75e089b7d367`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54c240903607e7bfceb958126e8c5cd48214de9e97b4d67528d4e108f6b613e`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37` - linux; ppc64le

```console
$ docker pull mariadb@sha256:86839d9106cbab2f4ee05188ba1c4240b825978621fa3427a97df903410bd759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116018747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5737a561d5c314f5bc83542d0b66f608b8e1380bf6b45269072764e566a14f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 16:30:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 16:32:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:32:39 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 16:33:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 16:34:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 16:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 16:34:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 16:34:47 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 16:34:52 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 16:35:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 16:38:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 16:38:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 16:38:57 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:39:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 16:39:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:39:17 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 16:39:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855e1295dc26a0c9b74e4482407b555044126c274cf25d14a488b5ac4cb2bc2`  
		Last Modified: Fri, 26 Mar 2021 16:47:30 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abddac719dc870aff20cad4f746209f976a1313fc6cd4f59f48df1e5584cf9`  
		Last Modified: Fri, 26 Mar 2021 16:47:32 GMT  
		Size: 5.6 MB (5630341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d763841542bc8c30fad86aca6afadc38ca331054204137f760297438be1e067`  
		Last Modified: Fri, 26 Mar 2021 16:47:31 GMT  
		Size: 1.2 MB (1246971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6807c27a6f6e0149bb26f56402a780b429982e4c3f8094b552ac3754c49a832`  
		Last Modified: Fri, 26 Mar 2021 16:47:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427969943d1691cb07a5bf70b1643649abc5bc2f42d5caf89f78f72f9a52d94`  
		Last Modified: Fri, 26 Mar 2021 16:47:27 GMT  
		Size: 934.9 KB (934923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240458af14f0c26fc73c4df8188481166204069bcdb39c5cb497fb5b98992280`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be7dd9df0131fba73b62e4a14056357bcb7eff9ee05e08a6b5a45ca8cb06a3`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8796b8c85e511e6d96632891801fc8335b04888982374bc30b96b31bec375496`  
		Last Modified: Fri, 26 Mar 2021 16:47:41 GMT  
		Size: 77.8 MB (77769530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc538d9d2381f73dd75c49b34017a1f2ccf08b96ba7aaaee50b2645d821985c`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312d5019b3781430c4e0ce58958ec15a58cee9035d9cd429dcc9e7960c9c9fa7`  
		Last Modified: Fri, 26 Mar 2021 16:47:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.37-bionic`

```console
$ docker pull mariadb@sha256:087f643fad1d66e868a27018e033ede151020ce2e327ddc988e49d6ee22db9b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.37-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:f70fbb0afeafb3a04d51650605ace81fa236c27fafa48b41b76d2c6485431359
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107995675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d6a130fc1fe1f83cfa7e55ab0165ad0f8f52d7c3900385ab75339bc6def686`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:52:16 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 11:52:46 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:52:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 11:53:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 11:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:53:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 11:53:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 11:53:32 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 11:53:32 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 11:53:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 11:54:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 11:54:21 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 11:54:21 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:54:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 11:54:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:54:23 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 11:54:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3f45e3863066b787d78c4ec01b2c4e92f6d137ef4437c29e5e73bed988dfad`  
		Last Modified: Fri, 26 Mar 2021 11:58:09 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02067a8ae4d84924bc19cbfde579f9713406eb19c0d3f87c45986b8895b2714c`  
		Last Modified: Fri, 26 Mar 2021 11:58:08 GMT  
		Size: 4.8 MB (4812807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7473d439bc3664901f88139c6861a1e4956bcf1cf70d786bc82d4ba1cdaed2`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 1.3 MB (1326645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cf83317dcdddfe432c60f9d2cf1f771499ba40e22b33bfbbb84d20805fdbad`  
		Last Modified: Fri, 26 Mar 2021 11:58:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee69a83317a136ef536a3deba8e13698b96dbcf4c6012e0684e6277dc495223d`  
		Last Modified: Fri, 26 Mar 2021 11:58:07 GMT  
		Size: 932.4 KB (932437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794113981a4c21a389b894d6f7a52f01e0f0d813d017c61bd91e3e4bd4345620`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab47c6c83bc366ae30f4ad6e5ab8e0ceacf42f683d7d85d7e08527cf5518e07e`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206171cc1dd1d1ad0c19e8554e05f49409a4f50b6d7d12184343850960c2bb32`  
		Last Modified: Fri, 26 Mar 2021 11:58:21 GMT  
		Size: 74.2 MB (74199294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b18a9d2c285b7cff0a91f215beaa5587cad9ea79b10bc7db67771f46be621d`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e643e5ef37013d5efddc6e3d860f218c6c214d25a267116c0a015579af46c2a`  
		Last Modified: Fri, 26 Mar 2021 11:58:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:0eefbab6ec39ca851d787312bbfcaeac7e292708dbabadb3d8164b33f7d251e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103143249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:393378e6c691ca88bd380e1007ad74bac5c360876fa925ae0a719c0661fac6e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:17:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 14:17:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:00 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:18:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:18:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:18:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:18:39 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 14:18:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:18:43 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 14:18:44 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 14:18:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 14:19:42 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 14:19:46 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 14:19:47 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:19:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 14:19:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:19:52 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 14:19:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0531f1390e72fa0458c10d1ba9d70291a68a00c704cb777bc8761be2410925ff`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72819a073b5b56ccfeca252e766511185478741b4305af5c57136bf9ad22022a`  
		Last Modified: Fri, 26 Mar 2021 14:24:07 GMT  
		Size: 4.4 MB (4395449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca3c34ec85cf0e786eef18f3472109ebdcc4c3fe0bdc1d98375ee9717fd1c9f`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 1.3 MB (1263787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c024f04ce1ac2812c515c15e819057471ab1c1e93a6fab65ebe924abe9892c`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d05c8a0a6ab565b8b1686dda41f172ecd8a51fa391fcaea711d14d2e7a87fc`  
		Last Modified: Fri, 26 Mar 2021 14:24:06 GMT  
		Size: 925.4 KB (925365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8e152c889b8e6ed5cab4ac0b79280a47d4fd0b8f6f88a40f9d55f779a5973`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56594ae78dce4d478095518713b80e59c2eaf613b0df64f5c6c4f5e513ddca30`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6834e4c7d6cfaeed1aa24a41cebcc7fa5ef6ace81ce67476fd0a327cf1550c4`  
		Last Modified: Fri, 26 Mar 2021 14:24:23 GMT  
		Size: 72.8 MB (72812142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9a00e9a2f9c7edf717bd86fbe2c28f85388e702cbfcfbc5a3a75e089b7d367`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54c240903607e7bfceb958126e8c5cd48214de9e97b4d67528d4e108f6b613e`  
		Last Modified: Fri, 26 Mar 2021 14:24:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:86839d9106cbab2f4ee05188ba1c4240b825978621fa3427a97df903410bd759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116018747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5737a561d5c314f5bc83542d0b66f608b8e1380bf6b45269072764e566a14f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 25 Mar 2021 22:54:50 GMT
ADD file:16a7a25947f319127d6b6ca6c99ff4e36bc4112c64ed67d2678b949eea2ad7e9 in / 
# Thu, 25 Mar 2021 22:56:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:57:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:57:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:59:22 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 16:30:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 26 Mar 2021 16:32:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:32:39 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 16:33:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 16:34:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 16:34:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 26 Mar 2021 16:34:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 16:34:47 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 26 Mar 2021 16:34:52 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 26 Mar 2021 16:35:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 26 Mar 2021 16:38:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 26 Mar 2021 16:38:54 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Mar 2021 16:38:57 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 16:39:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 26 Mar 2021 16:39:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 16:39:17 GMT
EXPOSE 3306
# Fri, 26 Mar 2021 16:39:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ade347cf74df0ad62b82c57b0a6f0411ef9ecad9336a99c9e116ee5d1ff3d82`  
		Last Modified: Thu, 25 Mar 2021 23:15:40 GMT  
		Size: 30.4 MB (30423262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918394a3ae216a0c5018f2cb9895614a0b9689fca3efc24700f5e1b1866273ad`  
		Last Modified: Thu, 25 Mar 2021 23:15:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5795a499c24598e294527992a703053ab615879af048f3b809a3ad86141684d`  
		Last Modified: Thu, 25 Mar 2021 22:58:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855e1295dc26a0c9b74e4482407b555044126c274cf25d14a488b5ac4cb2bc2`  
		Last Modified: Fri, 26 Mar 2021 16:47:30 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abddac719dc870aff20cad4f746209f976a1313fc6cd4f59f48df1e5584cf9`  
		Last Modified: Fri, 26 Mar 2021 16:47:32 GMT  
		Size: 5.6 MB (5630341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d763841542bc8c30fad86aca6afadc38ca331054204137f760297438be1e067`  
		Last Modified: Fri, 26 Mar 2021 16:47:31 GMT  
		Size: 1.2 MB (1246971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6807c27a6f6e0149bb26f56402a780b429982e4c3f8094b552ac3754c49a832`  
		Last Modified: Fri, 26 Mar 2021 16:47:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427969943d1691cb07a5bf70b1643649abc5bc2f42d5caf89f78f72f9a52d94`  
		Last Modified: Fri, 26 Mar 2021 16:47:27 GMT  
		Size: 934.9 KB (934923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240458af14f0c26fc73c4df8188481166204069bcdb39c5cb497fb5b98992280`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be7dd9df0131fba73b62e4a14056357bcb7eff9ee05e08a6b5a45ca8cb06a3`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8796b8c85e511e6d96632891801fc8335b04888982374bc30b96b31bec375496`  
		Last Modified: Fri, 26 Mar 2021 16:47:41 GMT  
		Size: 77.8 MB (77769530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc538d9d2381f73dd75c49b34017a1f2ccf08b96ba7aaaee50b2645d821985c`  
		Last Modified: Fri, 26 Mar 2021 16:47:23 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312d5019b3781430c4e0ce58958ec15a58cee9035d9cd429dcc9e7960c9c9fa7`  
		Last Modified: Fri, 26 Mar 2021 16:47:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:741dd7772c733277a74585ba2e1e933c8ccf42fb9833042b680f9b55a6a06993
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:c11dc2a0ca0ddd1600c90fdaa6fa4788bd29e8a69e3a71bfe071f954d8670abd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118351985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df12bc811acd71a35706d993bfca2a54d541e03c0bb57908bb145ad5b47df14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:12:15 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 02:12:15 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 02:12:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:12:42 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:12:42 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:12:42 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:12:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 02:12:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:12:44 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:12:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8bd0781d30e435ccf522445b67e0dd1a7c175732ca388df465b0e71e65a852`  
		Last Modified: Sat, 03 Apr 2021 02:14:45 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a4216e79f81c8a1462f6133f78d6f3287b38025b1622f1c70ef5803da184c`  
		Last Modified: Sat, 03 Apr 2021 02:14:57 GMT  
		Size: 81.7 MB (81686679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f700b49e151ced08d506d07ceea4ddbd844b92ba733cf6dd7a9f88b32a3cef`  
		Last Modified: Sat, 03 Apr 2021 02:14:44 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5399f565fa53ffb053122a4329bd841e5bc06c6cf50a097be14f5d98b5fda41`  
		Last Modified: Sat, 03 Apr 2021 02:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f5cdd751ccdc9542476b56cffca5f387ebd7a648dc270114b4d2eff73aff1833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116039083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2baa887980d8d30447cd3b2a18b8387b9f0b1bd59b20122d6f8c47688e6ec2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:18:45 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 06:18:46 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 06:18:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:19:35 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:19:38 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:19:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:19:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:19:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:19:45 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:19:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b75aa4dee001e3d306df121340b3c2c6291ce196dda6f4db46deeb5e3b730`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cf389d6775a65c871dee23378bc490c5bfa4369f5318d3646d465f6949e56`  
		Last Modified: Sat, 03 Apr 2021 06:22:00 GMT  
		Size: 80.9 MB (80862432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ebac7246630d000dcd9b5b8461762687c79f08db107e9506c91b0a5167a778`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f30724ff6969e4611c4634d71f0c43770c5a96317e8628a6aa0d9e718d0d76`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e0cb72150e7f4615a357c8cb20ab1ac8577bbfbd71ecfddc8242f1124bfb1600
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128921482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f49cd050d2c7219e7a9252553be8acfe828e062bf137ec99235ffe2f0c6e2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:53:10 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 06:53:15 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 06:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:55:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:55:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:55:33 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:55:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:55:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:55:50 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:55:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ee30076842699d0d2056bc0b7a6f6c7bf3c6f36e9d39caa60daa2a3b3f03d2`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af10041760104d4b7b5249687046ea79df0aea1585df66e730be3f67e4793ddf`  
		Last Modified: Sat, 03 Apr 2021 06:58:13 GMT  
		Size: 86.4 MB (86437095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b7f79d896cdffd341f7df40b8970e0c3d0831dcbc5f9d2c50181f7a0ae4b9`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceae640206be30e74ecdf41a8422192bf08d6b060388e91a5266f8cafdf6db03`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:741dd7772c733277a74585ba2e1e933c8ccf42fb9833042b680f9b55a6a06993
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c11dc2a0ca0ddd1600c90fdaa6fa4788bd29e8a69e3a71bfe071f954d8670abd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118351985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df12bc811acd71a35706d993bfca2a54d541e03c0bb57908bb145ad5b47df14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:12:15 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 02:12:15 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 02:12:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:12:42 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:12:42 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:12:42 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:12:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 02:12:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:12:44 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:12:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8bd0781d30e435ccf522445b67e0dd1a7c175732ca388df465b0e71e65a852`  
		Last Modified: Sat, 03 Apr 2021 02:14:45 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a4216e79f81c8a1462f6133f78d6f3287b38025b1622f1c70ef5803da184c`  
		Last Modified: Sat, 03 Apr 2021 02:14:57 GMT  
		Size: 81.7 MB (81686679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f700b49e151ced08d506d07ceea4ddbd844b92ba733cf6dd7a9f88b32a3cef`  
		Last Modified: Sat, 03 Apr 2021 02:14:44 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5399f565fa53ffb053122a4329bd841e5bc06c6cf50a097be14f5d98b5fda41`  
		Last Modified: Sat, 03 Apr 2021 02:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f5cdd751ccdc9542476b56cffca5f387ebd7a648dc270114b4d2eff73aff1833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116039083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2baa887980d8d30447cd3b2a18b8387b9f0b1bd59b20122d6f8c47688e6ec2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:18:45 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 06:18:46 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 06:18:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:19:35 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:19:38 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:19:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:19:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:19:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:19:45 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:19:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b75aa4dee001e3d306df121340b3c2c6291ce196dda6f4db46deeb5e3b730`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cf389d6775a65c871dee23378bc490c5bfa4369f5318d3646d465f6949e56`  
		Last Modified: Sat, 03 Apr 2021 06:22:00 GMT  
		Size: 80.9 MB (80862432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ebac7246630d000dcd9b5b8461762687c79f08db107e9506c91b0a5167a778`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f30724ff6969e4611c4634d71f0c43770c5a96317e8628a6aa0d9e718d0d76`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e0cb72150e7f4615a357c8cb20ab1ac8577bbfbd71ecfddc8242f1124bfb1600
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128921482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f49cd050d2c7219e7a9252553be8acfe828e062bf137ec99235ffe2f0c6e2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:53:10 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 06:53:15 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 06:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:55:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:55:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:55:33 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:55:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:55:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:55:50 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:55:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ee30076842699d0d2056bc0b7a6f6c7bf3c6f36e9d39caa60daa2a3b3f03d2`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af10041760104d4b7b5249687046ea79df0aea1585df66e730be3f67e4793ddf`  
		Last Modified: Sat, 03 Apr 2021 06:58:13 GMT  
		Size: 86.4 MB (86437095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b7f79d896cdffd341f7df40b8970e0c3d0831dcbc5f9d2c50181f7a0ae4b9`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceae640206be30e74ecdf41a8422192bf08d6b060388e91a5266f8cafdf6db03`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.28`

```console
$ docker pull mariadb@sha256:741dd7772c733277a74585ba2e1e933c8ccf42fb9833042b680f9b55a6a06993
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.28` - linux; amd64

```console
$ docker pull mariadb@sha256:c11dc2a0ca0ddd1600c90fdaa6fa4788bd29e8a69e3a71bfe071f954d8670abd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118351985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df12bc811acd71a35706d993bfca2a54d541e03c0bb57908bb145ad5b47df14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:12:15 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 02:12:15 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 02:12:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:12:42 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:12:42 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:12:42 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:12:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 02:12:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:12:44 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:12:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8bd0781d30e435ccf522445b67e0dd1a7c175732ca388df465b0e71e65a852`  
		Last Modified: Sat, 03 Apr 2021 02:14:45 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a4216e79f81c8a1462f6133f78d6f3287b38025b1622f1c70ef5803da184c`  
		Last Modified: Sat, 03 Apr 2021 02:14:57 GMT  
		Size: 81.7 MB (81686679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f700b49e151ced08d506d07ceea4ddbd844b92ba733cf6dd7a9f88b32a3cef`  
		Last Modified: Sat, 03 Apr 2021 02:14:44 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5399f565fa53ffb053122a4329bd841e5bc06c6cf50a097be14f5d98b5fda41`  
		Last Modified: Sat, 03 Apr 2021 02:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f5cdd751ccdc9542476b56cffca5f387ebd7a648dc270114b4d2eff73aff1833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116039083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2baa887980d8d30447cd3b2a18b8387b9f0b1bd59b20122d6f8c47688e6ec2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:18:45 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 06:18:46 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 06:18:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:19:35 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:19:38 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:19:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:19:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:19:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:19:45 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:19:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b75aa4dee001e3d306df121340b3c2c6291ce196dda6f4db46deeb5e3b730`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cf389d6775a65c871dee23378bc490c5bfa4369f5318d3646d465f6949e56`  
		Last Modified: Sat, 03 Apr 2021 06:22:00 GMT  
		Size: 80.9 MB (80862432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ebac7246630d000dcd9b5b8461762687c79f08db107e9506c91b0a5167a778`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f30724ff6969e4611c4634d71f0c43770c5a96317e8628a6aa0d9e718d0d76`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e0cb72150e7f4615a357c8cb20ab1ac8577bbfbd71ecfddc8242f1124bfb1600
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128921482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f49cd050d2c7219e7a9252553be8acfe828e062bf137ec99235ffe2f0c6e2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:53:10 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 06:53:15 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 06:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:55:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:55:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:55:33 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:55:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:55:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:55:50 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:55:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ee30076842699d0d2056bc0b7a6f6c7bf3c6f36e9d39caa60daa2a3b3f03d2`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af10041760104d4b7b5249687046ea79df0aea1585df66e730be3f67e4793ddf`  
		Last Modified: Sat, 03 Apr 2021 06:58:13 GMT  
		Size: 86.4 MB (86437095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b7f79d896cdffd341f7df40b8970e0c3d0831dcbc5f9d2c50181f7a0ae4b9`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceae640206be30e74ecdf41a8422192bf08d6b060388e91a5266f8cafdf6db03`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.28-focal`

```console
$ docker pull mariadb@sha256:741dd7772c733277a74585ba2e1e933c8ccf42fb9833042b680f9b55a6a06993
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.28-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c11dc2a0ca0ddd1600c90fdaa6fa4788bd29e8a69e3a71bfe071f954d8670abd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118351985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df12bc811acd71a35706d993bfca2a54d541e03c0bb57908bb145ad5b47df14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:12:15 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 02:12:15 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 02:12:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:12:42 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:12:42 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:12:42 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:12:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 02:12:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:12:44 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:12:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8bd0781d30e435ccf522445b67e0dd1a7c175732ca388df465b0e71e65a852`  
		Last Modified: Sat, 03 Apr 2021 02:14:45 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89a4216e79f81c8a1462f6133f78d6f3287b38025b1622f1c70ef5803da184c`  
		Last Modified: Sat, 03 Apr 2021 02:14:57 GMT  
		Size: 81.7 MB (81686679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f700b49e151ced08d506d07ceea4ddbd844b92ba733cf6dd7a9f88b32a3cef`  
		Last Modified: Sat, 03 Apr 2021 02:14:44 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5399f565fa53ffb053122a4329bd841e5bc06c6cf50a097be14f5d98b5fda41`  
		Last Modified: Sat, 03 Apr 2021 02:14:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f5cdd751ccdc9542476b56cffca5f387ebd7a648dc270114b4d2eff73aff1833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116039083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2baa887980d8d30447cd3b2a18b8387b9f0b1bd59b20122d6f8c47688e6ec2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:18:45 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 06:18:46 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 06:18:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:19:35 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:19:38 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:19:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:19:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:19:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:19:45 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:19:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1b75aa4dee001e3d306df121340b3c2c6291ce196dda6f4db46deeb5e3b730`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20cf389d6775a65c871dee23378bc490c5bfa4369f5318d3646d465f6949e56`  
		Last Modified: Sat, 03 Apr 2021 06:22:00 GMT  
		Size: 80.9 MB (80862432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ebac7246630d000dcd9b5b8461762687c79f08db107e9506c91b0a5167a778`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f30724ff6969e4611c4634d71f0c43770c5a96317e8628a6aa0d9e718d0d76`  
		Last Modified: Sat, 03 Apr 2021 06:21:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e0cb72150e7f4615a357c8cb20ab1ac8577bbfbd71ecfddc8242f1124bfb1600
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128921482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f49cd050d2c7219e7a9252553be8acfe828e062bf137ec99235ffe2f0c6e2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:53:10 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 03 Apr 2021 06:53:15 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 03 Apr 2021 06:53:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:55:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:55:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:55:33 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:55:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:55:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:55:50 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:55:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ee30076842699d0d2056bc0b7a6f6c7bf3c6f36e9d39caa60daa2a3b3f03d2`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af10041760104d4b7b5249687046ea79df0aea1585df66e730be3f67e4793ddf`  
		Last Modified: Sat, 03 Apr 2021 06:58:13 GMT  
		Size: 86.4 MB (86437095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1b7f79d896cdffd341f7df40b8970e0c3d0831dcbc5f9d2c50181f7a0ae4b9`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceae640206be30e74ecdf41a8422192bf08d6b060388e91a5266f8cafdf6db03`  
		Last Modified: Sat, 03 Apr 2021 06:57:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:2b392f05e34d689d26ac0a713abab1ffa3e74c2001f347b80696ed0223e38e1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:e54f5439f03e0067b4574494eabad064e750fc02567276d4c30da3a00da28a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122224437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb24818ad7354a54089e4562e12611992b257c13ebfc0d3d11d9382331538b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:11:39 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 02:11:39 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 02:11:40 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:12:04 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:12:05 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:12:05 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:12:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 02:12:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:12:07 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:12:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5b89a5e2a49e9ecc28453a8572cf762de78f5b6daa9c56bcce78c4717a5fd6`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80750bf4572669a160bf6d14e13e1f8e51d20d67016bd4e33fb42733888f548`  
		Last Modified: Sat, 03 Apr 2021 02:14:27 GMT  
		Size: 85.6 MB (85559128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f076592a5a7c5e8be12fb94ba3a8123ce674d36a6af16bb7c3e3fe11b9f9b972`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba1191135faa8c842f28d5c1cf6c0681a00778dd381f2bb4802344c55fcaa06`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8a135eb1f53fe3ea8569fb150885b0d2a67a6e62e5f30dcdb47c6bc6267e8847
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119807567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08cf720cfb37bfb61e6db62f429af9fb51bee91625234de69fb1b82448d6a416`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:17:47 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 06:17:48 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 06:17:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:18:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:18:30 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:18:31 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:18:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:18:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:18:35 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:18:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d68ffb5deffd16f762cde86a99382e264096eac9b33dcb0942b140b8024ae`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40bbb34628102783bd2e34e1f989d5367bf0eef6798f23ada3af9c1ea682439`  
		Last Modified: Sat, 03 Apr 2021 06:21:25 GMT  
		Size: 84.6 MB (84630917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68be439b0404aa9b498c1182efa1669932071e68557b1f7400199290b4574324`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf9a212cad527d0fc628615b5d2db4f7adb51045857baf47f58fdf04da92ee3`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a6d9c4efbefcc7f534985c9a481840af04b52cc8f9e2144ae241b44012c568de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132601087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1449973d5ee429a6136d2326addc5a7482132f03b8b88448ba340b3fc518cfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:50:00 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 06:50:03 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 06:50:18 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:52:33 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:52:39 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:52:42 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:52:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:52:57 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:53:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1b88fc289ab1fee0e6cec9d55ac7e220f92c52e7172dde5e136bd46ddead5`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e4c9d6faa150934ae430c2a0e9b47e52e2829b2391064b15073f7ecdedb9d5`  
		Last Modified: Sat, 03 Apr 2021 06:57:36 GMT  
		Size: 90.1 MB (90116703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69db86b9d22ed7a350cddc9897c2efb92fc393980f2c2684f2ff285f8f085be`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e53495bdda508dfda35254b94ad3cc795f81b65defab69c6645caadc4f47f`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:2b392f05e34d689d26ac0a713abab1ffa3e74c2001f347b80696ed0223e38e1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:e54f5439f03e0067b4574494eabad064e750fc02567276d4c30da3a00da28a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122224437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb24818ad7354a54089e4562e12611992b257c13ebfc0d3d11d9382331538b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:11:39 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 02:11:39 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 02:11:40 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:12:04 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:12:05 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:12:05 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:12:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 02:12:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:12:07 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:12:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5b89a5e2a49e9ecc28453a8572cf762de78f5b6daa9c56bcce78c4717a5fd6`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80750bf4572669a160bf6d14e13e1f8e51d20d67016bd4e33fb42733888f548`  
		Last Modified: Sat, 03 Apr 2021 02:14:27 GMT  
		Size: 85.6 MB (85559128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f076592a5a7c5e8be12fb94ba3a8123ce674d36a6af16bb7c3e3fe11b9f9b972`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba1191135faa8c842f28d5c1cf6c0681a00778dd381f2bb4802344c55fcaa06`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8a135eb1f53fe3ea8569fb150885b0d2a67a6e62e5f30dcdb47c6bc6267e8847
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119807567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08cf720cfb37bfb61e6db62f429af9fb51bee91625234de69fb1b82448d6a416`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:17:47 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 06:17:48 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 06:17:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:18:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:18:30 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:18:31 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:18:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:18:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:18:35 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:18:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d68ffb5deffd16f762cde86a99382e264096eac9b33dcb0942b140b8024ae`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40bbb34628102783bd2e34e1f989d5367bf0eef6798f23ada3af9c1ea682439`  
		Last Modified: Sat, 03 Apr 2021 06:21:25 GMT  
		Size: 84.6 MB (84630917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68be439b0404aa9b498c1182efa1669932071e68557b1f7400199290b4574324`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf9a212cad527d0fc628615b5d2db4f7adb51045857baf47f58fdf04da92ee3`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a6d9c4efbefcc7f534985c9a481840af04b52cc8f9e2144ae241b44012c568de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132601087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1449973d5ee429a6136d2326addc5a7482132f03b8b88448ba340b3fc518cfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:50:00 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 06:50:03 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 06:50:18 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:52:33 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:52:39 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:52:42 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:52:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:52:57 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:53:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1b88fc289ab1fee0e6cec9d55ac7e220f92c52e7172dde5e136bd46ddead5`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e4c9d6faa150934ae430c2a0e9b47e52e2829b2391064b15073f7ecdedb9d5`  
		Last Modified: Sat, 03 Apr 2021 06:57:36 GMT  
		Size: 90.1 MB (90116703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69db86b9d22ed7a350cddc9897c2efb92fc393980f2c2684f2ff285f8f085be`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e53495bdda508dfda35254b94ad3cc795f81b65defab69c6645caadc4f47f`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.18`

```console
$ docker pull mariadb@sha256:2b392f05e34d689d26ac0a713abab1ffa3e74c2001f347b80696ed0223e38e1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.18` - linux; amd64

```console
$ docker pull mariadb@sha256:e54f5439f03e0067b4574494eabad064e750fc02567276d4c30da3a00da28a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122224437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb24818ad7354a54089e4562e12611992b257c13ebfc0d3d11d9382331538b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:11:39 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 02:11:39 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 02:11:40 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:12:04 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:12:05 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:12:05 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:12:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 02:12:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:12:07 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:12:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5b89a5e2a49e9ecc28453a8572cf762de78f5b6daa9c56bcce78c4717a5fd6`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80750bf4572669a160bf6d14e13e1f8e51d20d67016bd4e33fb42733888f548`  
		Last Modified: Sat, 03 Apr 2021 02:14:27 GMT  
		Size: 85.6 MB (85559128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f076592a5a7c5e8be12fb94ba3a8123ce674d36a6af16bb7c3e3fe11b9f9b972`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba1191135faa8c842f28d5c1cf6c0681a00778dd381f2bb4802344c55fcaa06`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8a135eb1f53fe3ea8569fb150885b0d2a67a6e62e5f30dcdb47c6bc6267e8847
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119807567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08cf720cfb37bfb61e6db62f429af9fb51bee91625234de69fb1b82448d6a416`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:17:47 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 06:17:48 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 06:17:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:18:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:18:30 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:18:31 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:18:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:18:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:18:35 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:18:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d68ffb5deffd16f762cde86a99382e264096eac9b33dcb0942b140b8024ae`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40bbb34628102783bd2e34e1f989d5367bf0eef6798f23ada3af9c1ea682439`  
		Last Modified: Sat, 03 Apr 2021 06:21:25 GMT  
		Size: 84.6 MB (84630917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68be439b0404aa9b498c1182efa1669932071e68557b1f7400199290b4574324`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf9a212cad527d0fc628615b5d2db4f7adb51045857baf47f58fdf04da92ee3`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a6d9c4efbefcc7f534985c9a481840af04b52cc8f9e2144ae241b44012c568de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132601087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1449973d5ee429a6136d2326addc5a7482132f03b8b88448ba340b3fc518cfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:50:00 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 06:50:03 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 06:50:18 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:52:33 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:52:39 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:52:42 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:52:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:52:57 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:53:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1b88fc289ab1fee0e6cec9d55ac7e220f92c52e7172dde5e136bd46ddead5`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e4c9d6faa150934ae430c2a0e9b47e52e2829b2391064b15073f7ecdedb9d5`  
		Last Modified: Sat, 03 Apr 2021 06:57:36 GMT  
		Size: 90.1 MB (90116703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69db86b9d22ed7a350cddc9897c2efb92fc393980f2c2684f2ff285f8f085be`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e53495bdda508dfda35254b94ad3cc795f81b65defab69c6645caadc4f47f`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.18-focal`

```console
$ docker pull mariadb@sha256:2b392f05e34d689d26ac0a713abab1ffa3e74c2001f347b80696ed0223e38e1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.18-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:e54f5439f03e0067b4574494eabad064e750fc02567276d4c30da3a00da28a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122224437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb24818ad7354a54089e4562e12611992b257c13ebfc0d3d11d9382331538b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:11:39 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 02:11:39 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 02:11:40 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:12:04 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:12:05 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:12:05 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:12:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 02:12:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:12:07 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:12:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5b89a5e2a49e9ecc28453a8572cf762de78f5b6daa9c56bcce78c4717a5fd6`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80750bf4572669a160bf6d14e13e1f8e51d20d67016bd4e33fb42733888f548`  
		Last Modified: Sat, 03 Apr 2021 02:14:27 GMT  
		Size: 85.6 MB (85559128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f076592a5a7c5e8be12fb94ba3a8123ce674d36a6af16bb7c3e3fe11b9f9b972`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba1191135faa8c842f28d5c1cf6c0681a00778dd381f2bb4802344c55fcaa06`  
		Last Modified: Sat, 03 Apr 2021 02:14:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:8a135eb1f53fe3ea8569fb150885b0d2a67a6e62e5f30dcdb47c6bc6267e8847
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119807567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08cf720cfb37bfb61e6db62f429af9fb51bee91625234de69fb1b82448d6a416`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:17:47 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 06:17:48 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 06:17:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:18:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:18:30 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:18:31 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:18:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:18:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:18:35 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:18:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d68ffb5deffd16f762cde86a99382e264096eac9b33dcb0942b140b8024ae`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40bbb34628102783bd2e34e1f989d5367bf0eef6798f23ada3af9c1ea682439`  
		Last Modified: Sat, 03 Apr 2021 06:21:25 GMT  
		Size: 84.6 MB (84630917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68be439b0404aa9b498c1182efa1669932071e68557b1f7400199290b4574324`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf9a212cad527d0fc628615b5d2db4f7adb51045857baf47f58fdf04da92ee3`  
		Last Modified: Sat, 03 Apr 2021 06:21:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a6d9c4efbefcc7f534985c9a481840af04b52cc8f9e2144ae241b44012c568de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132601087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1449973d5ee429a6136d2326addc5a7482132f03b8b88448ba340b3fc518cfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:50:00 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 03 Apr 2021 06:50:03 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 03 Apr 2021 06:50:18 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:52:33 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:52:39 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:52:42 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:52:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 03 Apr 2021 06:52:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:52:57 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:53:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1b88fc289ab1fee0e6cec9d55ac7e220f92c52e7172dde5e136bd46ddead5`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e4c9d6faa150934ae430c2a0e9b47e52e2829b2391064b15073f7ecdedb9d5`  
		Last Modified: Sat, 03 Apr 2021 06:57:36 GMT  
		Size: 90.1 MB (90116703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69db86b9d22ed7a350cddc9897c2efb92fc393980f2c2684f2ff285f8f085be`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e53495bdda508dfda35254b94ad3cc795f81b65defab69c6645caadc4f47f`  
		Last Modified: Sat, 03 Apr 2021 06:57:17 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:9c681cefe72e257c6d58f839bb504f50bf259a0221c883fcc220f0755563fa46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:7e244fae615587335176db07e88b43eee5e4762f35306e17c13c68125d93b9bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124241217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76a4b2ed1b4014a9d638e15cd852544d8171c64ed78096fbe6e5a108fbf20b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:10:52 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 02:10:53 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 02:10:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:11:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:11:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:11:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:11:29 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:11:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f7bd4f1dda333860d0a1f30b5b8ec7ccedc7ea29bd90ba2b4cbc140f33c917`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5fa137d06e3953eab13f7fef4842cd2dcc883e398734c3ea923e9cc07a9ba`  
		Last Modified: Sat, 03 Apr 2021 02:13:37 GMT  
		Size: 87.6 MB (87576029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689a8c518900165fdb845e49162bbf561a2b291c79d6a7894e708a346c89ad74`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d4472cbcdcf08008f6be1e9d9a6e29f45aaead4cd0b4a6f4d0f7fb2892c9405
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121829873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43019a6fb0a9efab56424e9ce622b3aef9bf8505a4d51c7224f693a13d28a35d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:16:44 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:16:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:16:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:17:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:17:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:17:29 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:17:31 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:17:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e54de3da7dca0d12e5ba0bd3d6c00ed5f108cb341616aad40d750573525df`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72028e2877e63ed0d1ce1715663f908df19ca9beccce8e73c99e562d8a407b68`  
		Last Modified: Sat, 03 Apr 2021 06:20:47 GMT  
		Size: 86.7 MB (86653343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccaecdca9673211f0541464c67f03a0644842841e5cb8732d12ca0e804898b`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d2488fa0b439fae0630b2e7a8e757e8b6880afef3a20a004d39412f843655b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5a7472b0afafe37dbcff0a2e0db9ca30709f80d72bb941a056767f4e4d3f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:46:50 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:46:52 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:47:01 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:49:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:49:33 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:49:35 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:49:46 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:49:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a8ee527e9b195d270b34ff2ad5f33c81881e47c418b31a9dfd4fa359c72ec`  
		Last Modified: Sat, 03 Apr 2021 06:56:28 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3afa066a85db4a586c20e129f1dfdc7628d02e8f4d20a686e1d6a09f6fbae77`  
		Last Modified: Sat, 03 Apr 2021 06:56:49 GMT  
		Size: 92.2 MB (92198189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35002fcf886609f778e9c9844a7d94cc3a599a788b71339781f76f743df3fcba`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:9c681cefe72e257c6d58f839bb504f50bf259a0221c883fcc220f0755563fa46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7e244fae615587335176db07e88b43eee5e4762f35306e17c13c68125d93b9bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124241217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76a4b2ed1b4014a9d638e15cd852544d8171c64ed78096fbe6e5a108fbf20b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:10:52 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 02:10:53 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 02:10:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:11:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:11:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:11:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:11:29 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:11:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f7bd4f1dda333860d0a1f30b5b8ec7ccedc7ea29bd90ba2b4cbc140f33c917`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5fa137d06e3953eab13f7fef4842cd2dcc883e398734c3ea923e9cc07a9ba`  
		Last Modified: Sat, 03 Apr 2021 02:13:37 GMT  
		Size: 87.6 MB (87576029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689a8c518900165fdb845e49162bbf561a2b291c79d6a7894e708a346c89ad74`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d4472cbcdcf08008f6be1e9d9a6e29f45aaead4cd0b4a6f4d0f7fb2892c9405
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121829873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43019a6fb0a9efab56424e9ce622b3aef9bf8505a4d51c7224f693a13d28a35d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:16:44 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:16:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:16:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:17:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:17:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:17:29 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:17:31 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:17:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e54de3da7dca0d12e5ba0bd3d6c00ed5f108cb341616aad40d750573525df`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72028e2877e63ed0d1ce1715663f908df19ca9beccce8e73c99e562d8a407b68`  
		Last Modified: Sat, 03 Apr 2021 06:20:47 GMT  
		Size: 86.7 MB (86653343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccaecdca9673211f0541464c67f03a0644842841e5cb8732d12ca0e804898b`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d2488fa0b439fae0630b2e7a8e757e8b6880afef3a20a004d39412f843655b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5a7472b0afafe37dbcff0a2e0db9ca30709f80d72bb941a056767f4e4d3f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:46:50 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:46:52 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:47:01 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:49:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:49:33 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:49:35 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:49:46 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:49:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a8ee527e9b195d270b34ff2ad5f33c81881e47c418b31a9dfd4fa359c72ec`  
		Last Modified: Sat, 03 Apr 2021 06:56:28 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3afa066a85db4a586c20e129f1dfdc7628d02e8f4d20a686e1d6a09f6fbae77`  
		Last Modified: Sat, 03 Apr 2021 06:56:49 GMT  
		Size: 92.2 MB (92198189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35002fcf886609f778e9c9844a7d94cc3a599a788b71339781f76f743df3fcba`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.9`

```console
$ docker pull mariadb@sha256:9c681cefe72e257c6d58f839bb504f50bf259a0221c883fcc220f0755563fa46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.9` - linux; amd64

```console
$ docker pull mariadb@sha256:7e244fae615587335176db07e88b43eee5e4762f35306e17c13c68125d93b9bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124241217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76a4b2ed1b4014a9d638e15cd852544d8171c64ed78096fbe6e5a108fbf20b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:10:52 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 02:10:53 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 02:10:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:11:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:11:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:11:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:11:29 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:11:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f7bd4f1dda333860d0a1f30b5b8ec7ccedc7ea29bd90ba2b4cbc140f33c917`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5fa137d06e3953eab13f7fef4842cd2dcc883e398734c3ea923e9cc07a9ba`  
		Last Modified: Sat, 03 Apr 2021 02:13:37 GMT  
		Size: 87.6 MB (87576029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689a8c518900165fdb845e49162bbf561a2b291c79d6a7894e708a346c89ad74`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d4472cbcdcf08008f6be1e9d9a6e29f45aaead4cd0b4a6f4d0f7fb2892c9405
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121829873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43019a6fb0a9efab56424e9ce622b3aef9bf8505a4d51c7224f693a13d28a35d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:16:44 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:16:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:16:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:17:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:17:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:17:29 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:17:31 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:17:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e54de3da7dca0d12e5ba0bd3d6c00ed5f108cb341616aad40d750573525df`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72028e2877e63ed0d1ce1715663f908df19ca9beccce8e73c99e562d8a407b68`  
		Last Modified: Sat, 03 Apr 2021 06:20:47 GMT  
		Size: 86.7 MB (86653343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccaecdca9673211f0541464c67f03a0644842841e5cb8732d12ca0e804898b`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d2488fa0b439fae0630b2e7a8e757e8b6880afef3a20a004d39412f843655b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5a7472b0afafe37dbcff0a2e0db9ca30709f80d72bb941a056767f4e4d3f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:46:50 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:46:52 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:47:01 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:49:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:49:33 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:49:35 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:49:46 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:49:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a8ee527e9b195d270b34ff2ad5f33c81881e47c418b31a9dfd4fa359c72ec`  
		Last Modified: Sat, 03 Apr 2021 06:56:28 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3afa066a85db4a586c20e129f1dfdc7628d02e8f4d20a686e1d6a09f6fbae77`  
		Last Modified: Sat, 03 Apr 2021 06:56:49 GMT  
		Size: 92.2 MB (92198189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35002fcf886609f778e9c9844a7d94cc3a599a788b71339781f76f743df3fcba`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.9-focal`

```console
$ docker pull mariadb@sha256:9c681cefe72e257c6d58f839bb504f50bf259a0221c883fcc220f0755563fa46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.9-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7e244fae615587335176db07e88b43eee5e4762f35306e17c13c68125d93b9bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124241217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76a4b2ed1b4014a9d638e15cd852544d8171c64ed78096fbe6e5a108fbf20b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:10:52 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 02:10:53 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 02:10:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:11:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:11:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:11:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:11:29 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:11:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f7bd4f1dda333860d0a1f30b5b8ec7ccedc7ea29bd90ba2b4cbc140f33c917`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5fa137d06e3953eab13f7fef4842cd2dcc883e398734c3ea923e9cc07a9ba`  
		Last Modified: Sat, 03 Apr 2021 02:13:37 GMT  
		Size: 87.6 MB (87576029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689a8c518900165fdb845e49162bbf561a2b291c79d6a7894e708a346c89ad74`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d4472cbcdcf08008f6be1e9d9a6e29f45aaead4cd0b4a6f4d0f7fb2892c9405
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121829873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43019a6fb0a9efab56424e9ce622b3aef9bf8505a4d51c7224f693a13d28a35d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:16:44 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:16:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:16:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:17:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:17:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:17:29 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:17:31 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:17:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e54de3da7dca0d12e5ba0bd3d6c00ed5f108cb341616aad40d750573525df`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72028e2877e63ed0d1ce1715663f908df19ca9beccce8e73c99e562d8a407b68`  
		Last Modified: Sat, 03 Apr 2021 06:20:47 GMT  
		Size: 86.7 MB (86653343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccaecdca9673211f0541464c67f03a0644842841e5cb8732d12ca0e804898b`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d2488fa0b439fae0630b2e7a8e757e8b6880afef3a20a004d39412f843655b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5a7472b0afafe37dbcff0a2e0db9ca30709f80d72bb941a056767f4e4d3f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:46:50 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:46:52 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:47:01 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:49:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:49:33 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:49:35 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:49:46 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:49:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a8ee527e9b195d270b34ff2ad5f33c81881e47c418b31a9dfd4fa359c72ec`  
		Last Modified: Sat, 03 Apr 2021 06:56:28 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3afa066a85db4a586c20e129f1dfdc7628d02e8f4d20a686e1d6a09f6fbae77`  
		Last Modified: Sat, 03 Apr 2021 06:56:49 GMT  
		Size: 92.2 MB (92198189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35002fcf886609f778e9c9844a7d94cc3a599a788b71339781f76f743df3fcba`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:9c681cefe72e257c6d58f839bb504f50bf259a0221c883fcc220f0755563fa46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:7e244fae615587335176db07e88b43eee5e4762f35306e17c13c68125d93b9bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124241217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76a4b2ed1b4014a9d638e15cd852544d8171c64ed78096fbe6e5a108fbf20b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:10:52 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 02:10:53 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 02:10:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:11:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:11:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:11:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:11:29 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:11:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f7bd4f1dda333860d0a1f30b5b8ec7ccedc7ea29bd90ba2b4cbc140f33c917`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5fa137d06e3953eab13f7fef4842cd2dcc883e398734c3ea923e9cc07a9ba`  
		Last Modified: Sat, 03 Apr 2021 02:13:37 GMT  
		Size: 87.6 MB (87576029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689a8c518900165fdb845e49162bbf561a2b291c79d6a7894e708a346c89ad74`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d4472cbcdcf08008f6be1e9d9a6e29f45aaead4cd0b4a6f4d0f7fb2892c9405
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121829873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43019a6fb0a9efab56424e9ce622b3aef9bf8505a4d51c7224f693a13d28a35d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:16:44 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:16:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:16:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:17:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:17:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:17:29 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:17:31 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:17:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e54de3da7dca0d12e5ba0bd3d6c00ed5f108cb341616aad40d750573525df`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72028e2877e63ed0d1ce1715663f908df19ca9beccce8e73c99e562d8a407b68`  
		Last Modified: Sat, 03 Apr 2021 06:20:47 GMT  
		Size: 86.7 MB (86653343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccaecdca9673211f0541464c67f03a0644842841e5cb8732d12ca0e804898b`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d2488fa0b439fae0630b2e7a8e757e8b6880afef3a20a004d39412f843655b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5a7472b0afafe37dbcff0a2e0db9ca30709f80d72bb941a056767f4e4d3f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:46:50 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:46:52 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:47:01 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:49:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:49:33 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:49:35 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:49:46 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:49:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a8ee527e9b195d270b34ff2ad5f33c81881e47c418b31a9dfd4fa359c72ec`  
		Last Modified: Sat, 03 Apr 2021 06:56:28 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3afa066a85db4a586c20e129f1dfdc7628d02e8f4d20a686e1d6a09f6fbae77`  
		Last Modified: Sat, 03 Apr 2021 06:56:49 GMT  
		Size: 92.2 MB (92198189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35002fcf886609f778e9c9844a7d94cc3a599a788b71339781f76f743df3fcba`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:9c681cefe72e257c6d58f839bb504f50bf259a0221c883fcc220f0755563fa46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:7e244fae615587335176db07e88b43eee5e4762f35306e17c13c68125d93b9bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124241217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76a4b2ed1b4014a9d638e15cd852544d8171c64ed78096fbe6e5a108fbf20b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 02:10:28 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 02:10:35 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:35 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 02:10:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 02:10:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 02:10:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 02:10:51 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 02:10:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 02:10:52 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 02:10:53 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 02:10:54 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 02:11:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 02:11:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 02:11:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 02:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 02:11:29 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 02:11:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee25b525863cacdca61f8817dbbeca0112a7a1260c796b96868cac92348bb15`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bac9accf1550b3621fda1e695da9bd3d9d0fc7605909ef47d8bd99e7bcf5c7`  
		Last Modified: Sat, 03 Apr 2021 02:13:25 GMT  
		Size: 5.5 MB (5488871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553d41e82b111ab471ed2498f102daea01e0ee1e10f87f6eb680a7365482a26`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 1.3 MB (1324861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df5d11e950230d018577807901a95cb76531049bce96cd277d251bab15353dd`  
		Last Modified: Sat, 03 Apr 2021 02:13:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61f99a83efed351d96bfdb8029442c5feb987aab4cd58df1702f48bfc762a24`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 1.3 MB (1271662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd69eaf869090eba3eef0a98b6ce15c101e22c23bd33d0f5ac95c24996377c2`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 2.5 KB (2487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f7bd4f1dda333860d0a1f30b5b8ec7ccedc7ea29bd90ba2b4cbc140f33c917`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5fa137d06e3953eab13f7fef4842cd2dcc883e398734c3ea923e9cc07a9ba`  
		Last Modified: Sat, 03 Apr 2021 02:13:37 GMT  
		Size: 87.6 MB (87576029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689a8c518900165fdb845e49162bbf561a2b291c79d6a7894e708a346c89ad74`  
		Last Modified: Sat, 03 Apr 2021 02:13:21 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:5d4472cbcdcf08008f6be1e9d9a6e29f45aaead4cd0b4a6f4d0f7fb2892c9405
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121829873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43019a6fb0a9efab56424e9ce622b3aef9bf8505a4d51c7224f693a13d28a35d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:15:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:16:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:08 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:16:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:16:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:16:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:16:40 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:16:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:16:44 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:16:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:16:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:17:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:17:28 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:17:29 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:17:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:17:31 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:17:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df23206867a99978712fc27bb6697e9672cb5c31c8f4dd0b2bab1b86f39961f`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513810715d273575f5f627cf6504c637bba048d8594bfb4974be7df49859a19e`  
		Last Modified: Sat, 03 Apr 2021 06:20:27 GMT  
		Size: 5.5 MB (5455611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4083afdc3408dabb9575d9603ce4d8fe000410f112c044a922f39e81059e0a3`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 1.3 MB (1262203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0630d036c63617b35591d2b0e330ed792a00ccdbe7bc08abb8d07f64ca345b`  
		Last Modified: Sat, 03 Apr 2021 06:20:26 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770bd2f39de3d13899e90a6e006c9ad27f6935bd5b82ab9e10bf2d7fc99b6470`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 1.3 MB (1271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0b831035c5c14257cc3f282ec799ae298b2702eb4329b40575378e7e8d128`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e54de3da7dca0d12e5ba0bd3d6c00ed5f108cb341616aad40d750573525df`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72028e2877e63ed0d1ce1715663f908df19ca9beccce8e73c99e562d8a407b68`  
		Last Modified: Sat, 03 Apr 2021 06:20:47 GMT  
		Size: 86.7 MB (86653343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccaecdca9673211f0541464c67f03a0644842841e5cb8732d12ca0e804898b`  
		Last Modified: Sat, 03 Apr 2021 06:20:24 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4d2488fa0b439fae0630b2e7a8e757e8b6880afef3a20a004d39412f843655b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5a7472b0afafe37dbcff0a2e0db9ca30709f80d72bb941a056767f4e4d3f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:44:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 03 Apr 2021 06:45:16 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:45:21 GMT
ENV GOSU_VERSION=1.12
# Sat, 03 Apr 2021 06:46:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 03 Apr 2021 06:46:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 03 Apr 2021 06:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:46:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 03 Apr 2021 06:46:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 03 Apr 2021 06:46:50 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 03 Apr 2021 06:46:52 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 03 Apr 2021 06:47:01 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 03 Apr 2021 06:49:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 03 Apr 2021 06:49:33 GMT
VOLUME [/var/lib/mysql]
# Sat, 03 Apr 2021 06:49:35 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 03 Apr 2021 06:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Apr 2021 06:49:46 GMT
EXPOSE 3306
# Sat, 03 Apr 2021 06:49:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f34d606579c13ae31497ee0d9f15059085ebbd5d4953487332a9aa66e1d7a00`  
		Last Modified: Sat, 03 Apr 2021 06:56:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e712669eef0765f70e25bb7d9ffa17a0c164ef90c5d1410baea4d8a530a65702`  
		Last Modified: Sat, 03 Apr 2021 06:56:33 GMT  
		Size: 6.7 MB (6667932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0094e2d9450a4a4ab86bdf355c4d134f95040632ff887d3b0750f2403eba3`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 1.2 MB (1244481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28feeef0f33ff9f64dadbeace08615e4323d9ef94d588a1b99fb14a10fb8bac`  
		Last Modified: Sat, 03 Apr 2021 06:56:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0d664bfa964c8a4fb6bbab3c4211bce0a10365826c987801d629ea99fd688`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 1.3 MB (1281028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd51a69e14f5954c02386808c038b7f5191f413a87282ff29445b382d2727d4c`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a8ee527e9b195d270b34ff2ad5f33c81881e47c418b31a9dfd4fa359c72ec`  
		Last Modified: Sat, 03 Apr 2021 06:56:28 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3afa066a85db4a586c20e129f1dfdc7628d02e8f4d20a686e1d6a09f6fbae77`  
		Last Modified: Sat, 03 Apr 2021 06:56:49 GMT  
		Size: 92.2 MB (92198189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35002fcf886609f778e9c9844a7d94cc3a599a788b71339781f76f743df3fcba`  
		Last Modified: Sat, 03 Apr 2021 06:56:29 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
