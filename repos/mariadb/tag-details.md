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
$ docker pull mariadb@sha256:36288c675a192bd0a8a99cd6ba0780e31df85f0bfd0cbb204837cd108be3d236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:a362c0e1cffc6530e43e96e8bdd73d5735f3b5a7f4e1ae04667cf7285ca1ee1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124217165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992bce5ed7107642a27af59c2a2ddb7e589a44b639342b9501044511ab00aca0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 00:32:14 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:32:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:32:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:32:45 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:32:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:32:46 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:32:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a5dea1514db115cf28f9794262ca153c674751a11a39302a0ce3db6256c1d0`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5cf124c10ff33f1c7248e77e4ecaf76c89f19cdd826302c8ef54f2ac483ba`  
		Last Modified: Sat, 24 Apr 2021 00:36:47 GMT  
		Size: 87.6 MB (87577210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3352c2c9d21ce50c5af85c0fd16ddbed1a456eee52a5a34f44b465b7ff406281`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b01b1f9f4e04d4946c955b3e11a874f26791ca60cd305bda9999e43ca68be88c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121798059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9897eef8d73ac349375648c162a7b658565ed9a1a1dd36b6983adb19adccd5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:33:56 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 23 Apr 2021 23:33:57 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Fri, 23 Apr 2021 23:34:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:34:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:34:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:34:50 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:34:53 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:34:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf92de28cc1b694eb83365182205da153a31159d5d9ab06c67985100bd667ab`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb658d2a8224cd4532d094e05764d42def5d4974b2078d085c7c0d93a2d9056`  
		Last Modified: Fri, 23 Apr 2021 23:42:35 GMT  
		Size: 86.7 MB (86653573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34a83a38d8cdd7a6fe7f1ff714a32d6d452fab5f0bb34975b43ef2ceb99117`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:631c39535cd04a4614f510eb08d6a38edaa6155f1a793b0e6aee22249e6dfdd9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134658895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96625041fe6e55357b7eab093c0b90593fb9ef59c59bfc73b646ed4fb7a302de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:33 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 01:53:37 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 01:53:45 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:56:08 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:56:16 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:56:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:56:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:56:23 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3623b2360b0968a252476fb127f16f81174b3b9177234d78a4438374e6ff647`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58fb477779bd9749213f204c72c054541a404357cdc24fd2555478c8085c0b`  
		Last Modified: Sat, 24 Apr 2021 02:16:33 GMT  
		Size: 92.2 MB (92198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab7f51766b107f9d8e24502ceb64428358ff7c94d2742019b69259962d5f41`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:36288c675a192bd0a8a99cd6ba0780e31df85f0bfd0cbb204837cd108be3d236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a362c0e1cffc6530e43e96e8bdd73d5735f3b5a7f4e1ae04667cf7285ca1ee1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124217165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992bce5ed7107642a27af59c2a2ddb7e589a44b639342b9501044511ab00aca0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 00:32:14 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:32:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:32:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:32:45 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:32:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:32:46 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:32:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a5dea1514db115cf28f9794262ca153c674751a11a39302a0ce3db6256c1d0`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5cf124c10ff33f1c7248e77e4ecaf76c89f19cdd826302c8ef54f2ac483ba`  
		Last Modified: Sat, 24 Apr 2021 00:36:47 GMT  
		Size: 87.6 MB (87577210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3352c2c9d21ce50c5af85c0fd16ddbed1a456eee52a5a34f44b465b7ff406281`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b01b1f9f4e04d4946c955b3e11a874f26791ca60cd305bda9999e43ca68be88c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121798059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9897eef8d73ac349375648c162a7b658565ed9a1a1dd36b6983adb19adccd5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:33:56 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 23 Apr 2021 23:33:57 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Fri, 23 Apr 2021 23:34:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:34:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:34:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:34:50 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:34:53 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:34:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf92de28cc1b694eb83365182205da153a31159d5d9ab06c67985100bd667ab`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb658d2a8224cd4532d094e05764d42def5d4974b2078d085c7c0d93a2d9056`  
		Last Modified: Fri, 23 Apr 2021 23:42:35 GMT  
		Size: 86.7 MB (86653573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34a83a38d8cdd7a6fe7f1ff714a32d6d452fab5f0bb34975b43ef2ceb99117`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:631c39535cd04a4614f510eb08d6a38edaa6155f1a793b0e6aee22249e6dfdd9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134658895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96625041fe6e55357b7eab093c0b90593fb9ef59c59bfc73b646ed4fb7a302de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:33 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 01:53:37 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 01:53:45 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:56:08 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:56:16 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:56:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:56:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:56:23 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3623b2360b0968a252476fb127f16f81174b3b9177234d78a4438374e6ff647`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58fb477779bd9749213f204c72c054541a404357cdc24fd2555478c8085c0b`  
		Last Modified: Sat, 24 Apr 2021 02:16:33 GMT  
		Size: 92.2 MB (92198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab7f51766b107f9d8e24502ceb64428358ff7c94d2742019b69259962d5f41`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1`

```console
$ docker pull mariadb@sha256:1205b21b713812a6ba9fb59df206017dc06976fe68e172fbc6d153d7a4e13dfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1` - linux; amd64

```console
$ docker pull mariadb@sha256:bd44f3ef0bf4544a119732df8ffd038fec2992ff75435d03d6f1f142595f9020
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113174431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895244a22f379aaf1d942ddc5bf0769d717bedf2fe4056c10a24fc5daacf4229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:34:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:10 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:34:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:34:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:34:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:35:27 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 24 Apr 2021 00:35:27 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Sat, 24 Apr 2021 00:35:28 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:36:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:36:03 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:36:03 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:36:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:36:05 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:36:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3ea3a19e92c03376e50ab6be32a728766a9e215d3ac11a4fb63ea32d0057c`  
		Last Modified: Sat, 24 Apr 2021 00:38:29 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d9d23853df211590091594a2ff8e905b9981792837da1ebd3c3889bec3a3c`  
		Last Modified: Sat, 24 Apr 2021 00:38:30 GMT  
		Size: 4.8 MB (4814253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6512bf94537da3243c56c331eceacad34ca3d1f3119b52d882fcc655a3693cdc`  
		Last Modified: Sat, 24 Apr 2021 00:38:28 GMT  
		Size: 1.3 MB (1328139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75afd385b71debb0fb1b6ca3182dc7eb513bcce1efaaef0971b850e8a3b0c09`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1935952eac617e72d94f69becea58ac75a56f2e37437bc915eaaefbcd3adad`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 933.9 KB (933920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209bb6034896c057e2d27dda8c04b0b104b22e0aec7c5ec4e8dcc94ef2115d71`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa325c613ddbc109911fcaf2361190d40e9dff915417950ae15f5fc86aaf969e`  
		Last Modified: Sat, 24 Apr 2021 00:38:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050a67aa09dfcc73dee7bc2545aa7f20f66d597c7d68054e0fd20fd0010caa13`  
		Last Modified: Sat, 24 Apr 2021 00:39:08 GMT  
		Size: 79.4 MB (79387386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb7d28d54b6e45a5cd95de67dc46437c85888d4741b2d68de41f0a556cea606`  
		Last Modified: Sat, 24 Apr 2021 00:38:56 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc74f023b50c2c9286f81dc03284d6c7b2780df9705985aa5243c88142d1158`  
		Last Modified: Sat, 24 Apr 2021 00:38:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:7c4492d44fea3d10590d5870e1e24381fe583c93f241a6d453d7b1b5ebdb884d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105775436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b462edd5fd9d79d49da49236f7a5281da7274b39c2496e1e15049dda0cc4af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:37:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:38:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:38:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:38:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:38:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:58 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:39:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:40:28 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 23 Apr 2021 23:40:29 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 23 Apr 2021 23:40:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:41:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:41:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:41:30 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:41:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:41:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:41:35 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:41:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e3fb8fda77fd406c1841a586323c73d135e9e8418427fce79af8d4c7426cd9`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e44a4625823cdb75a2784347dec082934da2d2bdab7d36f70a3b3d8c3e272`  
		Last Modified: Fri, 23 Apr 2021 23:44:23 GMT  
		Size: 4.4 MB (4395643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2f23d2925988606a45c36359d8a9bf4f2b4c7a7d5d524f5474b074d574afe5`  
		Last Modified: Fri, 23 Apr 2021 23:44:22 GMT  
		Size: 1.3 MB (1263910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54945234d7c89f72cac10d09fd9d0ebcea488c96263f85fe451e333b551a87`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e0559b8697b3e56cce33d06f422df0baa7860f162b6ed44b42429017f3a64b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 925.5 KB (925512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee749c81d801a0a407f6b26b5777f53f9023af632dc98ca4a8285a92dcdba0f`  
		Last Modified: Fri, 23 Apr 2021 23:44:17 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367a9cdb7d1eda408321a9b6142a6c1efe300d89bc2586d4cf11dec080f93dc9`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f079a1652c9fba01644d55935a1002c531d0e7eb9e8918a404afe3d356fc240`  
		Last Modified: Fri, 23 Apr 2021 23:45:09 GMT  
		Size: 75.5 MB (75472954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf6bdaae6f60d6c42dc9a5c0803eae687dbfa36d7aa62fd19faf189e0093f9b`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c79a3e03a08a1aacc4ffde71603d8e97c9d70668a8f8820490048118bc3a6b`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; ppc64le

```console
$ docker pull mariadb@sha256:be227fc353e5d256d843960f4ff8a344b82776e9ff93f974389625eb9e547a18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118156992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76eba7ec8563ee56b2934a76122a31126b313c41da8277ece042797712575f2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:03:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 02:05:29 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:05:32 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 02:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 02:06:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 02:07:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:07:05 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 02:07:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:11:18 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 24 Apr 2021 02:11:21 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Sat, 24 Apr 2021 02:11:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:14:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:15:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:15:01 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:15:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:15:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:15:21 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:15:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea04cc788a73fbb77e77419e624d35468669efcc7e33b7a2a842b3c75fdd099a`  
		Last Modified: Sat, 24 Apr 2021 02:18:25 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc281e9316be7a239fa06bc2665e7e4bae49a243507e53c8aeb79fcdb502a0b8`  
		Last Modified: Sat, 24 Apr 2021 02:18:24 GMT  
		Size: 5.6 MB (5630381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e0f4fa75994be9888fa102801ee35060c21b8f36d166273260f5184a6520d`  
		Last Modified: Sat, 24 Apr 2021 02:18:23 GMT  
		Size: 1.2 MB (1246993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868afb3ea50f1c579aebff594111e079c5e1bfe45dbcccfe9e6e8c2b035b7f74`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec24e668bc60c8976ccc8c800e0b1316e40fdb30e63e5c39005d58ba4b2df4`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 934.9 KB (934939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670c55e77293fda2dc043a32c15066090a8179cd4e2ab5e2b0f10b2c23b590e`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14c15d5dbd9e0df534eb02395ab02f10c6cae22e809f620d0d1788dc633021c`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945b8207e313523ee2b68b1c9efd22ea60d4aedcc46ec5d96646c4161a6ffed9`  
		Last Modified: Sat, 24 Apr 2021 02:19:19 GMT  
		Size: 79.9 MB (79923644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d842d651dfe2b220fe92e911c7b0aa2b0c068fdb8c99dedd67a43f3b082cb1`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157a61a5b832cce311c81bb2c87bee287d87aea34c8e1e184fb8343ca857104c`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1-bionic`

```console
$ docker pull mariadb@sha256:1205b21b713812a6ba9fb59df206017dc06976fe68e172fbc6d153d7a4e13dfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:bd44f3ef0bf4544a119732df8ffd038fec2992ff75435d03d6f1f142595f9020
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113174431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895244a22f379aaf1d942ddc5bf0769d717bedf2fe4056c10a24fc5daacf4229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:34:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:10 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:34:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:34:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:34:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:35:27 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 24 Apr 2021 00:35:27 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Sat, 24 Apr 2021 00:35:28 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:36:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:36:03 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:36:03 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:36:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:36:05 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:36:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3ea3a19e92c03376e50ab6be32a728766a9e215d3ac11a4fb63ea32d0057c`  
		Last Modified: Sat, 24 Apr 2021 00:38:29 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d9d23853df211590091594a2ff8e905b9981792837da1ebd3c3889bec3a3c`  
		Last Modified: Sat, 24 Apr 2021 00:38:30 GMT  
		Size: 4.8 MB (4814253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6512bf94537da3243c56c331eceacad34ca3d1f3119b52d882fcc655a3693cdc`  
		Last Modified: Sat, 24 Apr 2021 00:38:28 GMT  
		Size: 1.3 MB (1328139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75afd385b71debb0fb1b6ca3182dc7eb513bcce1efaaef0971b850e8a3b0c09`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1935952eac617e72d94f69becea58ac75a56f2e37437bc915eaaefbcd3adad`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 933.9 KB (933920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209bb6034896c057e2d27dda8c04b0b104b22e0aec7c5ec4e8dcc94ef2115d71`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa325c613ddbc109911fcaf2361190d40e9dff915417950ae15f5fc86aaf969e`  
		Last Modified: Sat, 24 Apr 2021 00:38:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050a67aa09dfcc73dee7bc2545aa7f20f66d597c7d68054e0fd20fd0010caa13`  
		Last Modified: Sat, 24 Apr 2021 00:39:08 GMT  
		Size: 79.4 MB (79387386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb7d28d54b6e45a5cd95de67dc46437c85888d4741b2d68de41f0a556cea606`  
		Last Modified: Sat, 24 Apr 2021 00:38:56 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc74f023b50c2c9286f81dc03284d6c7b2780df9705985aa5243c88142d1158`  
		Last Modified: Sat, 24 Apr 2021 00:38:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:7c4492d44fea3d10590d5870e1e24381fe583c93f241a6d453d7b1b5ebdb884d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105775436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b462edd5fd9d79d49da49236f7a5281da7274b39c2496e1e15049dda0cc4af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:37:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:38:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:38:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:38:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:38:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:58 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:39:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:40:28 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 23 Apr 2021 23:40:29 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 23 Apr 2021 23:40:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:41:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:41:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:41:30 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:41:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:41:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:41:35 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:41:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e3fb8fda77fd406c1841a586323c73d135e9e8418427fce79af8d4c7426cd9`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e44a4625823cdb75a2784347dec082934da2d2bdab7d36f70a3b3d8c3e272`  
		Last Modified: Fri, 23 Apr 2021 23:44:23 GMT  
		Size: 4.4 MB (4395643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2f23d2925988606a45c36359d8a9bf4f2b4c7a7d5d524f5474b074d574afe5`  
		Last Modified: Fri, 23 Apr 2021 23:44:22 GMT  
		Size: 1.3 MB (1263910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54945234d7c89f72cac10d09fd9d0ebcea488c96263f85fe451e333b551a87`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e0559b8697b3e56cce33d06f422df0baa7860f162b6ed44b42429017f3a64b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 925.5 KB (925512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee749c81d801a0a407f6b26b5777f53f9023af632dc98ca4a8285a92dcdba0f`  
		Last Modified: Fri, 23 Apr 2021 23:44:17 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367a9cdb7d1eda408321a9b6142a6c1efe300d89bc2586d4cf11dec080f93dc9`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f079a1652c9fba01644d55935a1002c531d0e7eb9e8918a404afe3d356fc240`  
		Last Modified: Fri, 23 Apr 2021 23:45:09 GMT  
		Size: 75.5 MB (75472954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf6bdaae6f60d6c42dc9a5c0803eae687dbfa36d7aa62fd19faf189e0093f9b`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c79a3e03a08a1aacc4ffde71603d8e97c9d70668a8f8820490048118bc3a6b`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:be227fc353e5d256d843960f4ff8a344b82776e9ff93f974389625eb9e547a18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118156992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76eba7ec8563ee56b2934a76122a31126b313c41da8277ece042797712575f2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:03:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 02:05:29 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:05:32 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 02:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 02:06:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 02:07:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:07:05 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 02:07:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:11:18 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 24 Apr 2021 02:11:21 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Sat, 24 Apr 2021 02:11:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:14:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:15:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:15:01 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:15:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:15:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:15:21 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:15:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea04cc788a73fbb77e77419e624d35468669efcc7e33b7a2a842b3c75fdd099a`  
		Last Modified: Sat, 24 Apr 2021 02:18:25 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc281e9316be7a239fa06bc2665e7e4bae49a243507e53c8aeb79fcdb502a0b8`  
		Last Modified: Sat, 24 Apr 2021 02:18:24 GMT  
		Size: 5.6 MB (5630381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e0f4fa75994be9888fa102801ee35060c21b8f36d166273260f5184a6520d`  
		Last Modified: Sat, 24 Apr 2021 02:18:23 GMT  
		Size: 1.2 MB (1246993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868afb3ea50f1c579aebff594111e079c5e1bfe45dbcccfe9e6e8c2b035b7f74`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec24e668bc60c8976ccc8c800e0b1316e40fdb30e63e5c39005d58ba4b2df4`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 934.9 KB (934939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670c55e77293fda2dc043a32c15066090a8179cd4e2ab5e2b0f10b2c23b590e`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14c15d5dbd9e0df534eb02395ab02f10c6cae22e809f620d0d1788dc633021c`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945b8207e313523ee2b68b1c9efd22ea60d4aedcc46ec5d96646c4161a6ffed9`  
		Last Modified: Sat, 24 Apr 2021 02:19:19 GMT  
		Size: 79.9 MB (79923644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d842d651dfe2b220fe92e911c7b0aa2b0c068fdb8c99dedd67a43f3b082cb1`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157a61a5b832cce311c81bb2c87bee287d87aea34c8e1e184fb8343ca857104c`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48`

```console
$ docker pull mariadb@sha256:1205b21b713812a6ba9fb59df206017dc06976fe68e172fbc6d153d7a4e13dfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48` - linux; amd64

```console
$ docker pull mariadb@sha256:bd44f3ef0bf4544a119732df8ffd038fec2992ff75435d03d6f1f142595f9020
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113174431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895244a22f379aaf1d942ddc5bf0769d717bedf2fe4056c10a24fc5daacf4229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:34:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:10 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:34:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:34:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:34:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:35:27 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 24 Apr 2021 00:35:27 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Sat, 24 Apr 2021 00:35:28 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:36:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:36:03 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:36:03 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:36:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:36:05 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:36:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3ea3a19e92c03376e50ab6be32a728766a9e215d3ac11a4fb63ea32d0057c`  
		Last Modified: Sat, 24 Apr 2021 00:38:29 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d9d23853df211590091594a2ff8e905b9981792837da1ebd3c3889bec3a3c`  
		Last Modified: Sat, 24 Apr 2021 00:38:30 GMT  
		Size: 4.8 MB (4814253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6512bf94537da3243c56c331eceacad34ca3d1f3119b52d882fcc655a3693cdc`  
		Last Modified: Sat, 24 Apr 2021 00:38:28 GMT  
		Size: 1.3 MB (1328139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75afd385b71debb0fb1b6ca3182dc7eb513bcce1efaaef0971b850e8a3b0c09`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1935952eac617e72d94f69becea58ac75a56f2e37437bc915eaaefbcd3adad`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 933.9 KB (933920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209bb6034896c057e2d27dda8c04b0b104b22e0aec7c5ec4e8dcc94ef2115d71`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa325c613ddbc109911fcaf2361190d40e9dff915417950ae15f5fc86aaf969e`  
		Last Modified: Sat, 24 Apr 2021 00:38:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050a67aa09dfcc73dee7bc2545aa7f20f66d597c7d68054e0fd20fd0010caa13`  
		Last Modified: Sat, 24 Apr 2021 00:39:08 GMT  
		Size: 79.4 MB (79387386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb7d28d54b6e45a5cd95de67dc46437c85888d4741b2d68de41f0a556cea606`  
		Last Modified: Sat, 24 Apr 2021 00:38:56 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc74f023b50c2c9286f81dc03284d6c7b2780df9705985aa5243c88142d1158`  
		Last Modified: Sat, 24 Apr 2021 00:38:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:7c4492d44fea3d10590d5870e1e24381fe583c93f241a6d453d7b1b5ebdb884d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105775436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b462edd5fd9d79d49da49236f7a5281da7274b39c2496e1e15049dda0cc4af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:37:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:38:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:38:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:38:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:38:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:58 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:39:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:40:28 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 23 Apr 2021 23:40:29 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 23 Apr 2021 23:40:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:41:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:41:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:41:30 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:41:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:41:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:41:35 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:41:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e3fb8fda77fd406c1841a586323c73d135e9e8418427fce79af8d4c7426cd9`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e44a4625823cdb75a2784347dec082934da2d2bdab7d36f70a3b3d8c3e272`  
		Last Modified: Fri, 23 Apr 2021 23:44:23 GMT  
		Size: 4.4 MB (4395643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2f23d2925988606a45c36359d8a9bf4f2b4c7a7d5d524f5474b074d574afe5`  
		Last Modified: Fri, 23 Apr 2021 23:44:22 GMT  
		Size: 1.3 MB (1263910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54945234d7c89f72cac10d09fd9d0ebcea488c96263f85fe451e333b551a87`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e0559b8697b3e56cce33d06f422df0baa7860f162b6ed44b42429017f3a64b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 925.5 KB (925512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee749c81d801a0a407f6b26b5777f53f9023af632dc98ca4a8285a92dcdba0f`  
		Last Modified: Fri, 23 Apr 2021 23:44:17 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367a9cdb7d1eda408321a9b6142a6c1efe300d89bc2586d4cf11dec080f93dc9`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f079a1652c9fba01644d55935a1002c531d0e7eb9e8918a404afe3d356fc240`  
		Last Modified: Fri, 23 Apr 2021 23:45:09 GMT  
		Size: 75.5 MB (75472954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf6bdaae6f60d6c42dc9a5c0803eae687dbfa36d7aa62fd19faf189e0093f9b`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c79a3e03a08a1aacc4ffde71603d8e97c9d70668a8f8820490048118bc3a6b`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; ppc64le

```console
$ docker pull mariadb@sha256:be227fc353e5d256d843960f4ff8a344b82776e9ff93f974389625eb9e547a18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118156992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76eba7ec8563ee56b2934a76122a31126b313c41da8277ece042797712575f2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:03:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 02:05:29 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:05:32 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 02:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 02:06:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 02:07:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:07:05 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 02:07:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:11:18 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 24 Apr 2021 02:11:21 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Sat, 24 Apr 2021 02:11:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:14:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:15:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:15:01 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:15:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:15:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:15:21 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:15:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea04cc788a73fbb77e77419e624d35468669efcc7e33b7a2a842b3c75fdd099a`  
		Last Modified: Sat, 24 Apr 2021 02:18:25 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc281e9316be7a239fa06bc2665e7e4bae49a243507e53c8aeb79fcdb502a0b8`  
		Last Modified: Sat, 24 Apr 2021 02:18:24 GMT  
		Size: 5.6 MB (5630381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e0f4fa75994be9888fa102801ee35060c21b8f36d166273260f5184a6520d`  
		Last Modified: Sat, 24 Apr 2021 02:18:23 GMT  
		Size: 1.2 MB (1246993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868afb3ea50f1c579aebff594111e079c5e1bfe45dbcccfe9e6e8c2b035b7f74`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec24e668bc60c8976ccc8c800e0b1316e40fdb30e63e5c39005d58ba4b2df4`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 934.9 KB (934939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670c55e77293fda2dc043a32c15066090a8179cd4e2ab5e2b0f10b2c23b590e`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14c15d5dbd9e0df534eb02395ab02f10c6cae22e809f620d0d1788dc633021c`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945b8207e313523ee2b68b1c9efd22ea60d4aedcc46ec5d96646c4161a6ffed9`  
		Last Modified: Sat, 24 Apr 2021 02:19:19 GMT  
		Size: 79.9 MB (79923644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d842d651dfe2b220fe92e911c7b0aa2b0c068fdb8c99dedd67a43f3b082cb1`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157a61a5b832cce311c81bb2c87bee287d87aea34c8e1e184fb8343ca857104c`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48-bionic`

```console
$ docker pull mariadb@sha256:1205b21b713812a6ba9fb59df206017dc06976fe68e172fbc6d153d7a4e13dfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:bd44f3ef0bf4544a119732df8ffd038fec2992ff75435d03d6f1f142595f9020
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113174431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895244a22f379aaf1d942ddc5bf0769d717bedf2fe4056c10a24fc5daacf4229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:34:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:10 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:34:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:34:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:34:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:35:27 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 24 Apr 2021 00:35:27 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Sat, 24 Apr 2021 00:35:28 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:36:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:36:03 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:36:03 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:36:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:36:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:36:05 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:36:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3ea3a19e92c03376e50ab6be32a728766a9e215d3ac11a4fb63ea32d0057c`  
		Last Modified: Sat, 24 Apr 2021 00:38:29 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d9d23853df211590091594a2ff8e905b9981792837da1ebd3c3889bec3a3c`  
		Last Modified: Sat, 24 Apr 2021 00:38:30 GMT  
		Size: 4.8 MB (4814253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6512bf94537da3243c56c331eceacad34ca3d1f3119b52d882fcc655a3693cdc`  
		Last Modified: Sat, 24 Apr 2021 00:38:28 GMT  
		Size: 1.3 MB (1328139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75afd385b71debb0fb1b6ca3182dc7eb513bcce1efaaef0971b850e8a3b0c09`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1935952eac617e72d94f69becea58ac75a56f2e37437bc915eaaefbcd3adad`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 933.9 KB (933920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209bb6034896c057e2d27dda8c04b0b104b22e0aec7c5ec4e8dcc94ef2115d71`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa325c613ddbc109911fcaf2361190d40e9dff915417950ae15f5fc86aaf969e`  
		Last Modified: Sat, 24 Apr 2021 00:38:55 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050a67aa09dfcc73dee7bc2545aa7f20f66d597c7d68054e0fd20fd0010caa13`  
		Last Modified: Sat, 24 Apr 2021 00:39:08 GMT  
		Size: 79.4 MB (79387386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb7d28d54b6e45a5cd95de67dc46437c85888d4741b2d68de41f0a556cea606`  
		Last Modified: Sat, 24 Apr 2021 00:38:56 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc74f023b50c2c9286f81dc03284d6c7b2780df9705985aa5243c88142d1158`  
		Last Modified: Sat, 24 Apr 2021 00:38:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:7c4492d44fea3d10590d5870e1e24381fe583c93f241a6d453d7b1b5ebdb884d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105775436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b462edd5fd9d79d49da49236f7a5281da7274b39c2496e1e15049dda0cc4af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:37:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:38:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:38:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:38:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:38:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:58 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:39:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:40:28 GMT
ENV MARIADB_MAJOR=10.1
# Fri, 23 Apr 2021 23:40:29 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Fri, 23 Apr 2021 23:40:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:41:27 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:41:29 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:41:30 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:41:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:41:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:41:35 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:41:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e3fb8fda77fd406c1841a586323c73d135e9e8418427fce79af8d4c7426cd9`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e44a4625823cdb75a2784347dec082934da2d2bdab7d36f70a3b3d8c3e272`  
		Last Modified: Fri, 23 Apr 2021 23:44:23 GMT  
		Size: 4.4 MB (4395643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2f23d2925988606a45c36359d8a9bf4f2b4c7a7d5d524f5474b074d574afe5`  
		Last Modified: Fri, 23 Apr 2021 23:44:22 GMT  
		Size: 1.3 MB (1263910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54945234d7c89f72cac10d09fd9d0ebcea488c96263f85fe451e333b551a87`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e0559b8697b3e56cce33d06f422df0baa7860f162b6ed44b42429017f3a64b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 925.5 KB (925512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee749c81d801a0a407f6b26b5777f53f9023af632dc98ca4a8285a92dcdba0f`  
		Last Modified: Fri, 23 Apr 2021 23:44:17 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367a9cdb7d1eda408321a9b6142a6c1efe300d89bc2586d4cf11dec080f93dc9`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f079a1652c9fba01644d55935a1002c531d0e7eb9e8918a404afe3d356fc240`  
		Last Modified: Fri, 23 Apr 2021 23:45:09 GMT  
		Size: 75.5 MB (75472954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf6bdaae6f60d6c42dc9a5c0803eae687dbfa36d7aa62fd19faf189e0093f9b`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c79a3e03a08a1aacc4ffde71603d8e97c9d70668a8f8820490048118bc3a6b`  
		Last Modified: Fri, 23 Apr 2021 23:44:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:be227fc353e5d256d843960f4ff8a344b82776e9ff93f974389625eb9e547a18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118156992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76eba7ec8563ee56b2934a76122a31126b313c41da8277ece042797712575f2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:03:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 02:05:29 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:05:32 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 02:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 02:06:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 02:07:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:07:05 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 02:07:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:11:18 GMT
ENV MARIADB_MAJOR=10.1
# Sat, 24 Apr 2021 02:11:21 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Sat, 24 Apr 2021 02:11:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:14:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:15:00 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:15:01 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:15:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:15:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:15:21 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:15:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea04cc788a73fbb77e77419e624d35468669efcc7e33b7a2a842b3c75fdd099a`  
		Last Modified: Sat, 24 Apr 2021 02:18:25 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc281e9316be7a239fa06bc2665e7e4bae49a243507e53c8aeb79fcdb502a0b8`  
		Last Modified: Sat, 24 Apr 2021 02:18:24 GMT  
		Size: 5.6 MB (5630381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e0f4fa75994be9888fa102801ee35060c21b8f36d166273260f5184a6520d`  
		Last Modified: Sat, 24 Apr 2021 02:18:23 GMT  
		Size: 1.2 MB (1246993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868afb3ea50f1c579aebff594111e079c5e1bfe45dbcccfe9e6e8c2b035b7f74`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec24e668bc60c8976ccc8c800e0b1316e40fdb30e63e5c39005d58ba4b2df4`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 934.9 KB (934939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670c55e77293fda2dc043a32c15066090a8179cd4e2ab5e2b0f10b2c23b590e`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14c15d5dbd9e0df534eb02395ab02f10c6cae22e809f620d0d1788dc633021c`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945b8207e313523ee2b68b1c9efd22ea60d4aedcc46ec5d96646c4161a6ffed9`  
		Last Modified: Sat, 24 Apr 2021 02:19:19 GMT  
		Size: 79.9 MB (79923644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d842d651dfe2b220fe92e911c7b0aa2b0c068fdb8c99dedd67a43f3b082cb1`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157a61a5b832cce311c81bb2c87bee287d87aea34c8e1e184fb8343ca857104c`  
		Last Modified: Sat, 24 Apr 2021 02:19:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:55e33bf8866391f30f099a9933f6187f9699d8b896c1eab1df1c4621a9646be0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:7e335138f4b79e453846c56c2c46f2a7244f143bec8eb56e0100086f2b717c2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107987794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e280c5820040d570938102bc451f2916e7b2e35426a24e8c44b12079d902790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:34:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:10 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:34:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:34:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:34:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:34:29 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 24 Apr 2021 00:34:29 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Sat, 24 Apr 2021 00:34:30 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:35:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:35:11 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:35:12 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:35:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:35:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:35:13 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:35:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3ea3a19e92c03376e50ab6be32a728766a9e215d3ac11a4fb63ea32d0057c`  
		Last Modified: Sat, 24 Apr 2021 00:38:29 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d9d23853df211590091594a2ff8e905b9981792837da1ebd3c3889bec3a3c`  
		Last Modified: Sat, 24 Apr 2021 00:38:30 GMT  
		Size: 4.8 MB (4814253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6512bf94537da3243c56c331eceacad34ca3d1f3119b52d882fcc655a3693cdc`  
		Last Modified: Sat, 24 Apr 2021 00:38:28 GMT  
		Size: 1.3 MB (1328139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75afd385b71debb0fb1b6ca3182dc7eb513bcce1efaaef0971b850e8a3b0c09`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1935952eac617e72d94f69becea58ac75a56f2e37437bc915eaaefbcd3adad`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 933.9 KB (933920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209bb6034896c057e2d27dda8c04b0b104b22e0aec7c5ec4e8dcc94ef2115d71`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a193656db97c5bff1250c6def0d80ada6579fe8f33ce1b6123695cf7cc53cd94`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392397d32761ceaabfa2329e474a674359d3ceb148cd5fd47715d2a4bb1b612b`  
		Last Modified: Sat, 24 Apr 2021 00:38:36 GMT  
		Size: 74.2 MB (74200748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dab60bfc0f4d5d2e1cb822080b597c490f662affd9283e251bba1f8f0c7733`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.0 KB (5037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d69b7780e75b7709ec2c0583862e2cd2b3c90275708ee0b2f19331bd51c5c0`  
		Last Modified: Sat, 24 Apr 2021 00:38:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c8c3c33576ed682e7805a991e42736426fbacc5d18e190cb9e543e995fa5ce56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103114715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90f1613c960b838e656352f6a9b44ab3386a38f95d6dd72bdbf58081fc50eaa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:37:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:38:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:38:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:38:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:38:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:58 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:39:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:39:01 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 23 Apr 2021 23:39:01 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 23 Apr 2021 23:39:04 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:39:59 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:40:01 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:40:02 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:40:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:40:06 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e3fb8fda77fd406c1841a586323c73d135e9e8418427fce79af8d4c7426cd9`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e44a4625823cdb75a2784347dec082934da2d2bdab7d36f70a3b3d8c3e272`  
		Last Modified: Fri, 23 Apr 2021 23:44:23 GMT  
		Size: 4.4 MB (4395643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2f23d2925988606a45c36359d8a9bf4f2b4c7a7d5d524f5474b074d574afe5`  
		Last Modified: Fri, 23 Apr 2021 23:44:22 GMT  
		Size: 1.3 MB (1263910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54945234d7c89f72cac10d09fd9d0ebcea488c96263f85fe451e333b551a87`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e0559b8697b3e56cce33d06f422df0baa7860f162b6ed44b42429017f3a64b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 925.5 KB (925512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee749c81d801a0a407f6b26b5777f53f9023af632dc98ca4a8285a92dcdba0f`  
		Last Modified: Fri, 23 Apr 2021 23:44:17 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74f7865f3644e076ab2cfa2fa730aaab664c6445728f1acc79ab9737e435d4b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a24ddee3dfeeb3933933df9b6405b039a64a6c06c82ec8c98b269706a63841f`  
		Last Modified: Fri, 23 Apr 2021 23:44:36 GMT  
		Size: 72.8 MB (72812235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48516cc0cf08ce532d2b0adacbdb7b9813bd24abcce971ac827c9d820d76536b`  
		Last Modified: Fri, 23 Apr 2021 23:44:20 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06159d7910d4999d158d6a07290cc9c8c7d847dc7b4731e8cd835f2085e77440`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa637ab8dbd32da131d67d0562fadd2839ba0c99a450bafb99a2a07d6bb73c0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116003529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9fb0c04863bacc0a89e8740517cb99098fad9738f3142623bf91e4519a5acf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:03:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 02:05:29 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:05:32 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 02:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 02:06:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 02:07:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:07:05 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 02:07:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:07:23 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 24 Apr 2021 02:07:26 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Sat, 24 Apr 2021 02:07:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:10:32 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:10:41 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:10:43 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:10:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:11:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:11:06 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:11:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea04cc788a73fbb77e77419e624d35468669efcc7e33b7a2a842b3c75fdd099a`  
		Last Modified: Sat, 24 Apr 2021 02:18:25 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc281e9316be7a239fa06bc2665e7e4bae49a243507e53c8aeb79fcdb502a0b8`  
		Last Modified: Sat, 24 Apr 2021 02:18:24 GMT  
		Size: 5.6 MB (5630381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e0f4fa75994be9888fa102801ee35060c21b8f36d166273260f5184a6520d`  
		Last Modified: Sat, 24 Apr 2021 02:18:23 GMT  
		Size: 1.2 MB (1246993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868afb3ea50f1c579aebff594111e079c5e1bfe45dbcccfe9e6e8c2b035b7f74`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec24e668bc60c8976ccc8c800e0b1316e40fdb30e63e5c39005d58ba4b2df4`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 934.9 KB (934939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670c55e77293fda2dc043a32c15066090a8179cd4e2ab5e2b0f10b2c23b590e`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767030366176eb8f2b86ef8bc8e55c37bfda0c704df66063a89288929e726f13`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d743d937ff6e5f395ccdbd92ae8d6f981aaebb7b51cae7881dfe2c021cc2c8`  
		Last Modified: Sat, 24 Apr 2021 02:18:38 GMT  
		Size: 77.8 MB (77770180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e55f74b819b04920dcf1d0b327c953e76b9b4cd0280ea872e6b0ee9539fe62`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1cdc966658b53c4ad48b9866b27dde1fb0b7694fcf0aebbd34d4802e40e2c`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:55e33bf8866391f30f099a9933f6187f9699d8b896c1eab1df1c4621a9646be0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:7e335138f4b79e453846c56c2c46f2a7244f143bec8eb56e0100086f2b717c2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107987794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e280c5820040d570938102bc451f2916e7b2e35426a24e8c44b12079d902790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:34:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:10 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:34:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:34:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:34:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:34:29 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 24 Apr 2021 00:34:29 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Sat, 24 Apr 2021 00:34:30 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:35:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:35:11 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:35:12 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:35:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:35:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:35:13 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:35:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3ea3a19e92c03376e50ab6be32a728766a9e215d3ac11a4fb63ea32d0057c`  
		Last Modified: Sat, 24 Apr 2021 00:38:29 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d9d23853df211590091594a2ff8e905b9981792837da1ebd3c3889bec3a3c`  
		Last Modified: Sat, 24 Apr 2021 00:38:30 GMT  
		Size: 4.8 MB (4814253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6512bf94537da3243c56c331eceacad34ca3d1f3119b52d882fcc655a3693cdc`  
		Last Modified: Sat, 24 Apr 2021 00:38:28 GMT  
		Size: 1.3 MB (1328139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75afd385b71debb0fb1b6ca3182dc7eb513bcce1efaaef0971b850e8a3b0c09`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1935952eac617e72d94f69becea58ac75a56f2e37437bc915eaaefbcd3adad`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 933.9 KB (933920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209bb6034896c057e2d27dda8c04b0b104b22e0aec7c5ec4e8dcc94ef2115d71`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a193656db97c5bff1250c6def0d80ada6579fe8f33ce1b6123695cf7cc53cd94`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392397d32761ceaabfa2329e474a674359d3ceb148cd5fd47715d2a4bb1b612b`  
		Last Modified: Sat, 24 Apr 2021 00:38:36 GMT  
		Size: 74.2 MB (74200748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dab60bfc0f4d5d2e1cb822080b597c490f662affd9283e251bba1f8f0c7733`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.0 KB (5037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d69b7780e75b7709ec2c0583862e2cd2b3c90275708ee0b2f19331bd51c5c0`  
		Last Modified: Sat, 24 Apr 2021 00:38:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c8c3c33576ed682e7805a991e42736426fbacc5d18e190cb9e543e995fa5ce56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103114715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90f1613c960b838e656352f6a9b44ab3386a38f95d6dd72bdbf58081fc50eaa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:37:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:38:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:38:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:38:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:38:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:58 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:39:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:39:01 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 23 Apr 2021 23:39:01 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 23 Apr 2021 23:39:04 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:39:59 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:40:01 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:40:02 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:40:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:40:06 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e3fb8fda77fd406c1841a586323c73d135e9e8418427fce79af8d4c7426cd9`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e44a4625823cdb75a2784347dec082934da2d2bdab7d36f70a3b3d8c3e272`  
		Last Modified: Fri, 23 Apr 2021 23:44:23 GMT  
		Size: 4.4 MB (4395643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2f23d2925988606a45c36359d8a9bf4f2b4c7a7d5d524f5474b074d574afe5`  
		Last Modified: Fri, 23 Apr 2021 23:44:22 GMT  
		Size: 1.3 MB (1263910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54945234d7c89f72cac10d09fd9d0ebcea488c96263f85fe451e333b551a87`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e0559b8697b3e56cce33d06f422df0baa7860f162b6ed44b42429017f3a64b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 925.5 KB (925512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee749c81d801a0a407f6b26b5777f53f9023af632dc98ca4a8285a92dcdba0f`  
		Last Modified: Fri, 23 Apr 2021 23:44:17 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74f7865f3644e076ab2cfa2fa730aaab664c6445728f1acc79ab9737e435d4b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a24ddee3dfeeb3933933df9b6405b039a64a6c06c82ec8c98b269706a63841f`  
		Last Modified: Fri, 23 Apr 2021 23:44:36 GMT  
		Size: 72.8 MB (72812235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48516cc0cf08ce532d2b0adacbdb7b9813bd24abcce971ac827c9d820d76536b`  
		Last Modified: Fri, 23 Apr 2021 23:44:20 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06159d7910d4999d158d6a07290cc9c8c7d847dc7b4731e8cd835f2085e77440`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa637ab8dbd32da131d67d0562fadd2839ba0c99a450bafb99a2a07d6bb73c0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116003529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9fb0c04863bacc0a89e8740517cb99098fad9738f3142623bf91e4519a5acf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:03:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 02:05:29 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:05:32 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 02:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 02:06:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 02:07:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:07:05 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 02:07:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:07:23 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 24 Apr 2021 02:07:26 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Sat, 24 Apr 2021 02:07:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:10:32 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:10:41 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:10:43 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:10:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:11:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:11:06 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:11:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea04cc788a73fbb77e77419e624d35468669efcc7e33b7a2a842b3c75fdd099a`  
		Last Modified: Sat, 24 Apr 2021 02:18:25 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc281e9316be7a239fa06bc2665e7e4bae49a243507e53c8aeb79fcdb502a0b8`  
		Last Modified: Sat, 24 Apr 2021 02:18:24 GMT  
		Size: 5.6 MB (5630381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e0f4fa75994be9888fa102801ee35060c21b8f36d166273260f5184a6520d`  
		Last Modified: Sat, 24 Apr 2021 02:18:23 GMT  
		Size: 1.2 MB (1246993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868afb3ea50f1c579aebff594111e079c5e1bfe45dbcccfe9e6e8c2b035b7f74`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec24e668bc60c8976ccc8c800e0b1316e40fdb30e63e5c39005d58ba4b2df4`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 934.9 KB (934939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670c55e77293fda2dc043a32c15066090a8179cd4e2ab5e2b0f10b2c23b590e`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767030366176eb8f2b86ef8bc8e55c37bfda0c704df66063a89288929e726f13`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d743d937ff6e5f395ccdbd92ae8d6f981aaebb7b51cae7881dfe2c021cc2c8`  
		Last Modified: Sat, 24 Apr 2021 02:18:38 GMT  
		Size: 77.8 MB (77770180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e55f74b819b04920dcf1d0b327c953e76b9b4cd0280ea872e6b0ee9539fe62`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1cdc966658b53c4ad48b9866b27dde1fb0b7694fcf0aebbd34d4802e40e2c`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.37`

```console
$ docker pull mariadb@sha256:55e33bf8866391f30f099a9933f6187f9699d8b896c1eab1df1c4621a9646be0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.37` - linux; amd64

```console
$ docker pull mariadb@sha256:7e335138f4b79e453846c56c2c46f2a7244f143bec8eb56e0100086f2b717c2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107987794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e280c5820040d570938102bc451f2916e7b2e35426a24e8c44b12079d902790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:34:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:10 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:34:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:34:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:34:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:34:29 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 24 Apr 2021 00:34:29 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Sat, 24 Apr 2021 00:34:30 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:35:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:35:11 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:35:12 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:35:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:35:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:35:13 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:35:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3ea3a19e92c03376e50ab6be32a728766a9e215d3ac11a4fb63ea32d0057c`  
		Last Modified: Sat, 24 Apr 2021 00:38:29 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d9d23853df211590091594a2ff8e905b9981792837da1ebd3c3889bec3a3c`  
		Last Modified: Sat, 24 Apr 2021 00:38:30 GMT  
		Size: 4.8 MB (4814253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6512bf94537da3243c56c331eceacad34ca3d1f3119b52d882fcc655a3693cdc`  
		Last Modified: Sat, 24 Apr 2021 00:38:28 GMT  
		Size: 1.3 MB (1328139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75afd385b71debb0fb1b6ca3182dc7eb513bcce1efaaef0971b850e8a3b0c09`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1935952eac617e72d94f69becea58ac75a56f2e37437bc915eaaefbcd3adad`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 933.9 KB (933920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209bb6034896c057e2d27dda8c04b0b104b22e0aec7c5ec4e8dcc94ef2115d71`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a193656db97c5bff1250c6def0d80ada6579fe8f33ce1b6123695cf7cc53cd94`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392397d32761ceaabfa2329e474a674359d3ceb148cd5fd47715d2a4bb1b612b`  
		Last Modified: Sat, 24 Apr 2021 00:38:36 GMT  
		Size: 74.2 MB (74200748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dab60bfc0f4d5d2e1cb822080b597c490f662affd9283e251bba1f8f0c7733`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.0 KB (5037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d69b7780e75b7709ec2c0583862e2cd2b3c90275708ee0b2f19331bd51c5c0`  
		Last Modified: Sat, 24 Apr 2021 00:38:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c8c3c33576ed682e7805a991e42736426fbacc5d18e190cb9e543e995fa5ce56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103114715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90f1613c960b838e656352f6a9b44ab3386a38f95d6dd72bdbf58081fc50eaa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:37:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:38:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:38:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:38:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:38:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:58 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:39:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:39:01 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 23 Apr 2021 23:39:01 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 23 Apr 2021 23:39:04 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:39:59 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:40:01 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:40:02 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:40:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:40:06 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e3fb8fda77fd406c1841a586323c73d135e9e8418427fce79af8d4c7426cd9`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e44a4625823cdb75a2784347dec082934da2d2bdab7d36f70a3b3d8c3e272`  
		Last Modified: Fri, 23 Apr 2021 23:44:23 GMT  
		Size: 4.4 MB (4395643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2f23d2925988606a45c36359d8a9bf4f2b4c7a7d5d524f5474b074d574afe5`  
		Last Modified: Fri, 23 Apr 2021 23:44:22 GMT  
		Size: 1.3 MB (1263910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54945234d7c89f72cac10d09fd9d0ebcea488c96263f85fe451e333b551a87`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e0559b8697b3e56cce33d06f422df0baa7860f162b6ed44b42429017f3a64b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 925.5 KB (925512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee749c81d801a0a407f6b26b5777f53f9023af632dc98ca4a8285a92dcdba0f`  
		Last Modified: Fri, 23 Apr 2021 23:44:17 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74f7865f3644e076ab2cfa2fa730aaab664c6445728f1acc79ab9737e435d4b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a24ddee3dfeeb3933933df9b6405b039a64a6c06c82ec8c98b269706a63841f`  
		Last Modified: Fri, 23 Apr 2021 23:44:36 GMT  
		Size: 72.8 MB (72812235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48516cc0cf08ce532d2b0adacbdb7b9813bd24abcce971ac827c9d820d76536b`  
		Last Modified: Fri, 23 Apr 2021 23:44:20 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06159d7910d4999d158d6a07290cc9c8c7d847dc7b4731e8cd835f2085e77440`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa637ab8dbd32da131d67d0562fadd2839ba0c99a450bafb99a2a07d6bb73c0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116003529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9fb0c04863bacc0a89e8740517cb99098fad9738f3142623bf91e4519a5acf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:03:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 02:05:29 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:05:32 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 02:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 02:06:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 02:07:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:07:05 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 02:07:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:07:23 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 24 Apr 2021 02:07:26 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Sat, 24 Apr 2021 02:07:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:10:32 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:10:41 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:10:43 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:10:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:11:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:11:06 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:11:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea04cc788a73fbb77e77419e624d35468669efcc7e33b7a2a842b3c75fdd099a`  
		Last Modified: Sat, 24 Apr 2021 02:18:25 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc281e9316be7a239fa06bc2665e7e4bae49a243507e53c8aeb79fcdb502a0b8`  
		Last Modified: Sat, 24 Apr 2021 02:18:24 GMT  
		Size: 5.6 MB (5630381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e0f4fa75994be9888fa102801ee35060c21b8f36d166273260f5184a6520d`  
		Last Modified: Sat, 24 Apr 2021 02:18:23 GMT  
		Size: 1.2 MB (1246993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868afb3ea50f1c579aebff594111e079c5e1bfe45dbcccfe9e6e8c2b035b7f74`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec24e668bc60c8976ccc8c800e0b1316e40fdb30e63e5c39005d58ba4b2df4`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 934.9 KB (934939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670c55e77293fda2dc043a32c15066090a8179cd4e2ab5e2b0f10b2c23b590e`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767030366176eb8f2b86ef8bc8e55c37bfda0c704df66063a89288929e726f13`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d743d937ff6e5f395ccdbd92ae8d6f981aaebb7b51cae7881dfe2c021cc2c8`  
		Last Modified: Sat, 24 Apr 2021 02:18:38 GMT  
		Size: 77.8 MB (77770180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e55f74b819b04920dcf1d0b327c953e76b9b4cd0280ea872e6b0ee9539fe62`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1cdc966658b53c4ad48b9866b27dde1fb0b7694fcf0aebbd34d4802e40e2c`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.37-bionic`

```console
$ docker pull mariadb@sha256:55e33bf8866391f30f099a9933f6187f9699d8b896c1eab1df1c4621a9646be0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.37-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:7e335138f4b79e453846c56c2c46f2a7244f143bec8eb56e0100086f2b717c2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107987794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e280c5820040d570938102bc451f2916e7b2e35426a24e8c44b12079d902790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:22 GMT
ADD file:d7fa3c26651f9204a5629287a1a9a6e7dc6a0bc6eb499e82c433c0c8f67ff46b in / 
# Fri, 23 Apr 2021 22:21:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:25 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:34:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:34:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:10 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:34:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:34:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:34:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:34:28 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:34:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:34:29 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 24 Apr 2021 00:34:29 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Sat, 24 Apr 2021 00:34:30 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:35:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:35:11 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:35:12 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:35:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:35:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:35:13 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:35:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01bf7da0a88c9e37ae418d17c0aeed0621524848d80ccb9e38c67e7ab8e11928`  
		Last Modified: Fri, 16 Apr 2021 15:20:23 GMT  
		Size: 26.7 MB (26697009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b4a5f15c7a0722b4f22e61b5387317eaf2602c27ffb2bceac9a25f19fbd156`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ffbe87baa135002dddb7a7460082c5d6a352186e1be9464c5f31db81378824`  
		Last Modified: Fri, 23 Apr 2021 22:22:45 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3ea3a19e92c03376e50ab6be32a728766a9e215d3ac11a4fb63ea32d0057c`  
		Last Modified: Sat, 24 Apr 2021 00:38:29 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d9d23853df211590091594a2ff8e905b9981792837da1ebd3c3889bec3a3c`  
		Last Modified: Sat, 24 Apr 2021 00:38:30 GMT  
		Size: 4.8 MB (4814253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6512bf94537da3243c56c331eceacad34ca3d1f3119b52d882fcc655a3693cdc`  
		Last Modified: Sat, 24 Apr 2021 00:38:28 GMT  
		Size: 1.3 MB (1328139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75afd385b71debb0fb1b6ca3182dc7eb513bcce1efaaef0971b850e8a3b0c09`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1935952eac617e72d94f69becea58ac75a56f2e37437bc915eaaefbcd3adad`  
		Last Modified: Sat, 24 Apr 2021 00:38:27 GMT  
		Size: 933.9 KB (933920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209bb6034896c057e2d27dda8c04b0b104b22e0aec7c5ec4e8dcc94ef2115d71`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a193656db97c5bff1250c6def0d80ada6579fe8f33ce1b6123695cf7cc53cd94`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392397d32761ceaabfa2329e474a674359d3ceb148cd5fd47715d2a4bb1b612b`  
		Last Modified: Sat, 24 Apr 2021 00:38:36 GMT  
		Size: 74.2 MB (74200748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48dab60bfc0f4d5d2e1cb822080b597c490f662affd9283e251bba1f8f0c7733`  
		Last Modified: Sat, 24 Apr 2021 00:38:24 GMT  
		Size: 5.0 KB (5037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d69b7780e75b7709ec2c0583862e2cd2b3c90275708ee0b2f19331bd51c5c0`  
		Last Modified: Sat, 24 Apr 2021 00:38:26 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c8c3c33576ed682e7805a991e42736426fbacc5d18e190cb9e543e995fa5ce56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103114715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90f1613c960b838e656352f6a9b44ab3386a38f95d6dd72bdbf58081fc50eaa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:15 GMT
ADD file:5f7cb4b44f843eaef6ae7ddb75dfc228a33d20cd974074ca23c1bb2cad7f77ad in / 
# Fri, 23 Apr 2021 22:47:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:24 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:37:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:38:17 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:38:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:38:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:38:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:38:58 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:39:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:39:01 GMT
ENV MARIADB_MAJOR=10.2
# Fri, 23 Apr 2021 23:39:01 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Fri, 23 Apr 2021 23:39:04 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:39:59 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:40:01 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:40:02 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:40:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:40:06 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:40:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:673aeee5c81c892477834e2b5e55575f16bfd52d9b841a1d8c524fb3805ee960`  
		Last Modified: Fri, 16 Apr 2021 16:25:11 GMT  
		Size: 23.7 MB (23703698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b2790219d2003c0d437e634927887ee5cc3d8f985d7459adc5b2ff62d003f`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509c77ce92ade89fbf09fe03b167023be51bf5a0c14c00487fa7a9ee33b55fc3`  
		Last Modified: Fri, 23 Apr 2021 22:49:51 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e3fb8fda77fd406c1841a586323c73d135e9e8418427fce79af8d4c7426cd9`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e44a4625823cdb75a2784347dec082934da2d2bdab7d36f70a3b3d8c3e272`  
		Last Modified: Fri, 23 Apr 2021 23:44:23 GMT  
		Size: 4.4 MB (4395643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2f23d2925988606a45c36359d8a9bf4f2b4c7a7d5d524f5474b074d574afe5`  
		Last Modified: Fri, 23 Apr 2021 23:44:22 GMT  
		Size: 1.3 MB (1263910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54945234d7c89f72cac10d09fd9d0ebcea488c96263f85fe451e333b551a87`  
		Last Modified: Fri, 23 Apr 2021 23:44:21 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e0559b8697b3e56cce33d06f422df0baa7860f162b6ed44b42429017f3a64b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 925.5 KB (925512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee749c81d801a0a407f6b26b5777f53f9023af632dc98ca4a8285a92dcdba0f`  
		Last Modified: Fri, 23 Apr 2021 23:44:17 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74f7865f3644e076ab2cfa2fa730aaab664c6445728f1acc79ab9737e435d4b`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a24ddee3dfeeb3933933df9b6405b039a64a6c06c82ec8c98b269706a63841f`  
		Last Modified: Fri, 23 Apr 2021 23:44:36 GMT  
		Size: 72.8 MB (72812235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48516cc0cf08ce532d2b0adacbdb7b9813bd24abcce971ac827c9d820d76536b`  
		Last Modified: Fri, 23 Apr 2021 23:44:20 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06159d7910d4999d158d6a07290cc9c8c7d847dc7b4731e8cd835f2085e77440`  
		Last Modified: Fri, 23 Apr 2021 23:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:aa637ab8dbd32da131d67d0562fadd2839ba0c99a450bafb99a2a07d6bb73c0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116003529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9fb0c04863bacc0a89e8740517cb99098fad9738f3142623bf91e4519a5acf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:30:25 GMT
ADD file:818f810cd30ef74fd4690c6265d80265647ba3353880cf8323500df6d2c48b69 in / 
# Fri, 23 Apr 2021 22:30:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:31:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:31:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:31:32 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 02:03:43 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 02:05:29 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:05:32 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 02:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 02:06:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 02:07:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 02:07:05 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 02:07:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:07:23 GMT
ENV MARIADB_MAJOR=10.2
# Sat, 24 Apr 2021 02:07:26 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Sat, 24 Apr 2021 02:07:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:10:32 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:10:41 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:10:43 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:10:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:11:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:11:06 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:11:12 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb3095714506c08a64a49e29ab001d7000d94957d52e05db35361fd4a54c460c`  
		Last Modified: Fri, 23 Apr 2021 22:36:52 GMT  
		Size: 30.4 MB (30407300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd29acc6f7bfef8034eaca0bfb069f0d66e50351c84b062e224d6eae710afa79`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7645fc50c9e70df51732b36ef7f8b21ebacd148c3bee4f1b29ca6dcba1bbb949`  
		Last Modified: Fri, 23 Apr 2021 22:36:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea04cc788a73fbb77e77419e624d35468669efcc7e33b7a2a842b3c75fdd099a`  
		Last Modified: Sat, 24 Apr 2021 02:18:25 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc281e9316be7a239fa06bc2665e7e4bae49a243507e53c8aeb79fcdb502a0b8`  
		Last Modified: Sat, 24 Apr 2021 02:18:24 GMT  
		Size: 5.6 MB (5630381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13e0f4fa75994be9888fa102801ee35060c21b8f36d166273260f5184a6520d`  
		Last Modified: Sat, 24 Apr 2021 02:18:23 GMT  
		Size: 1.2 MB (1246993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868afb3ea50f1c579aebff594111e079c5e1bfe45dbcccfe9e6e8c2b035b7f74`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec24e668bc60c8976ccc8c800e0b1316e40fdb30e63e5c39005d58ba4b2df4`  
		Last Modified: Sat, 24 Apr 2021 02:18:22 GMT  
		Size: 934.9 KB (934939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670c55e77293fda2dc043a32c15066090a8179cd4e2ab5e2b0f10b2c23b590e`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767030366176eb8f2b86ef8bc8e55c37bfda0c704df66063a89288929e726f13`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d743d937ff6e5f395ccdbd92ae8d6f981aaebb7b51cae7881dfe2c021cc2c8`  
		Last Modified: Sat, 24 Apr 2021 02:18:38 GMT  
		Size: 77.8 MB (77770180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e55f74b819b04920dcf1d0b327c953e76b9b4cd0280ea872e6b0ee9539fe62`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c1cdc966658b53c4ad48b9866b27dde1fb0b7694fcf0aebbd34d4802e40e2c`  
		Last Modified: Sat, 24 Apr 2021 02:18:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:df7edb9de3ba069b6d5dfc4882798d11b401817a0d166d0f6076eb9865313920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:b5a051d8feaa86aed3d62b55d8ff5b457bb4754b5e7ba21e63d9ca4ccb3f5af7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118327915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512186ae7f53662017f42a73f8dd5ce822aacd9873b847f28a8ccf20868f4293`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:33:25 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 24 Apr 2021 00:33:25 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 24 Apr 2021 00:33:26 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:33:53 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:33:54 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:33:54 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:33:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:33:55 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:33:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7fc27a6a863a4620fc3da7c2aa4c8b4b2ee5fcca88f459cf0fedbdcd548fd4`  
		Last Modified: Sat, 24 Apr 2021 00:37:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04e45a90e173ff1f3ccfc630bea9526918dd0dc5a74a011819679fa0e29c885`  
		Last Modified: Sat, 24 Apr 2021 00:38:06 GMT  
		Size: 81.7 MB (81687842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc20c2d0927609ab8ac205f7f27cfc8194bf7993dbf2f9595e850862bc516250`  
		Last Modified: Sat, 24 Apr 2021 00:37:52 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e189f24a7dd6b6739c7a6110ba3fe8065f5208974dc4386cfed6426fef855b`  
		Last Modified: Sat, 24 Apr 2021 00:37:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4bd68304b338c591eb5aa39033826107013f44960d859a5f48d6268c0a605b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116006894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1887b121bf3b90fbcc249a1ebff3282f415a5f06c84eff80c0024c541bf4cbc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:36:34 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 23 Apr 2021 23:36:35 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Fri, 23 Apr 2021 23:36:41 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:37:29 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:37:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:37:32 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:37:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:37:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:37:36 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:37:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be52582cab73354a0e4d897c88d485858f8fa1dc98ec8e982faeb9dba19d9c2f`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8173267e77964d10ccb5049b81b0f4385e0af4e269c76841c0eba9080b813b`  
		Last Modified: Fri, 23 Apr 2021 23:44:06 GMT  
		Size: 80.9 MB (80862291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff99a2d812b02ad30fe65d4d74e60806e891cddc13ca8714feec8d6d8567df6`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971b6f235d6345df394933f34c380b68e8ebb0e6487f49246d3c45a1de3f04a9`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3dadd2ddf07aaa2418e09f614561c5b8151f081747de9c07b5b3cefd14cd18bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128898109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bc4cbb89eff87d0cb24e3c59a939e80ab6cf07bdd38129a70bda6b677385cef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:00:08 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 24 Apr 2021 02:00:12 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 24 Apr 2021 02:00:25 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:02:51 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:03:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:03:04 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:03:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:03:15 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:03:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd5d0d35665f927618341beedb67deb8837c42b6e358619057b9ca430db0d8e`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f89cd035af5eb9af324668b04fe04636f7ad396708f2d6dd431db2a853c53f9`  
		Last Modified: Sat, 24 Apr 2021 02:18:00 GMT  
		Size: 86.4 MB (86437537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f265070eaaf750af50c32c148cb64e8f1981928afd84eef382420271f9eea03`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 5.0 KB (5036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c92c233bf14760a22129e5c30a446df97f50b059c4f0b9c2dae8c921ffd9e7`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:df7edb9de3ba069b6d5dfc4882798d11b401817a0d166d0f6076eb9865313920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:b5a051d8feaa86aed3d62b55d8ff5b457bb4754b5e7ba21e63d9ca4ccb3f5af7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118327915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512186ae7f53662017f42a73f8dd5ce822aacd9873b847f28a8ccf20868f4293`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:33:25 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 24 Apr 2021 00:33:25 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 24 Apr 2021 00:33:26 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:33:53 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:33:54 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:33:54 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:33:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:33:55 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:33:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7fc27a6a863a4620fc3da7c2aa4c8b4b2ee5fcca88f459cf0fedbdcd548fd4`  
		Last Modified: Sat, 24 Apr 2021 00:37:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04e45a90e173ff1f3ccfc630bea9526918dd0dc5a74a011819679fa0e29c885`  
		Last Modified: Sat, 24 Apr 2021 00:38:06 GMT  
		Size: 81.7 MB (81687842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc20c2d0927609ab8ac205f7f27cfc8194bf7993dbf2f9595e850862bc516250`  
		Last Modified: Sat, 24 Apr 2021 00:37:52 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e189f24a7dd6b6739c7a6110ba3fe8065f5208974dc4386cfed6426fef855b`  
		Last Modified: Sat, 24 Apr 2021 00:37:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4bd68304b338c591eb5aa39033826107013f44960d859a5f48d6268c0a605b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116006894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1887b121bf3b90fbcc249a1ebff3282f415a5f06c84eff80c0024c541bf4cbc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:36:34 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 23 Apr 2021 23:36:35 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Fri, 23 Apr 2021 23:36:41 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:37:29 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:37:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:37:32 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:37:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:37:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:37:36 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:37:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be52582cab73354a0e4d897c88d485858f8fa1dc98ec8e982faeb9dba19d9c2f`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8173267e77964d10ccb5049b81b0f4385e0af4e269c76841c0eba9080b813b`  
		Last Modified: Fri, 23 Apr 2021 23:44:06 GMT  
		Size: 80.9 MB (80862291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff99a2d812b02ad30fe65d4d74e60806e891cddc13ca8714feec8d6d8567df6`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971b6f235d6345df394933f34c380b68e8ebb0e6487f49246d3c45a1de3f04a9`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3dadd2ddf07aaa2418e09f614561c5b8151f081747de9c07b5b3cefd14cd18bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128898109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bc4cbb89eff87d0cb24e3c59a939e80ab6cf07bdd38129a70bda6b677385cef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:00:08 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 24 Apr 2021 02:00:12 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 24 Apr 2021 02:00:25 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:02:51 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:03:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:03:04 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:03:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:03:15 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:03:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd5d0d35665f927618341beedb67deb8837c42b6e358619057b9ca430db0d8e`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f89cd035af5eb9af324668b04fe04636f7ad396708f2d6dd431db2a853c53f9`  
		Last Modified: Sat, 24 Apr 2021 02:18:00 GMT  
		Size: 86.4 MB (86437537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f265070eaaf750af50c32c148cb64e8f1981928afd84eef382420271f9eea03`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 5.0 KB (5036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c92c233bf14760a22129e5c30a446df97f50b059c4f0b9c2dae8c921ffd9e7`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.28`

```console
$ docker pull mariadb@sha256:df7edb9de3ba069b6d5dfc4882798d11b401817a0d166d0f6076eb9865313920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.28` - linux; amd64

```console
$ docker pull mariadb@sha256:b5a051d8feaa86aed3d62b55d8ff5b457bb4754b5e7ba21e63d9ca4ccb3f5af7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118327915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512186ae7f53662017f42a73f8dd5ce822aacd9873b847f28a8ccf20868f4293`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:33:25 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 24 Apr 2021 00:33:25 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 24 Apr 2021 00:33:26 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:33:53 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:33:54 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:33:54 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:33:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:33:55 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:33:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7fc27a6a863a4620fc3da7c2aa4c8b4b2ee5fcca88f459cf0fedbdcd548fd4`  
		Last Modified: Sat, 24 Apr 2021 00:37:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04e45a90e173ff1f3ccfc630bea9526918dd0dc5a74a011819679fa0e29c885`  
		Last Modified: Sat, 24 Apr 2021 00:38:06 GMT  
		Size: 81.7 MB (81687842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc20c2d0927609ab8ac205f7f27cfc8194bf7993dbf2f9595e850862bc516250`  
		Last Modified: Sat, 24 Apr 2021 00:37:52 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e189f24a7dd6b6739c7a6110ba3fe8065f5208974dc4386cfed6426fef855b`  
		Last Modified: Sat, 24 Apr 2021 00:37:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4bd68304b338c591eb5aa39033826107013f44960d859a5f48d6268c0a605b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116006894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1887b121bf3b90fbcc249a1ebff3282f415a5f06c84eff80c0024c541bf4cbc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:36:34 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 23 Apr 2021 23:36:35 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Fri, 23 Apr 2021 23:36:41 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:37:29 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:37:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:37:32 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:37:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:37:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:37:36 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:37:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be52582cab73354a0e4d897c88d485858f8fa1dc98ec8e982faeb9dba19d9c2f`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8173267e77964d10ccb5049b81b0f4385e0af4e269c76841c0eba9080b813b`  
		Last Modified: Fri, 23 Apr 2021 23:44:06 GMT  
		Size: 80.9 MB (80862291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff99a2d812b02ad30fe65d4d74e60806e891cddc13ca8714feec8d6d8567df6`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971b6f235d6345df394933f34c380b68e8ebb0e6487f49246d3c45a1de3f04a9`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3dadd2ddf07aaa2418e09f614561c5b8151f081747de9c07b5b3cefd14cd18bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128898109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bc4cbb89eff87d0cb24e3c59a939e80ab6cf07bdd38129a70bda6b677385cef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:00:08 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 24 Apr 2021 02:00:12 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 24 Apr 2021 02:00:25 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:02:51 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:03:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:03:04 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:03:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:03:15 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:03:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd5d0d35665f927618341beedb67deb8837c42b6e358619057b9ca430db0d8e`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f89cd035af5eb9af324668b04fe04636f7ad396708f2d6dd431db2a853c53f9`  
		Last Modified: Sat, 24 Apr 2021 02:18:00 GMT  
		Size: 86.4 MB (86437537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f265070eaaf750af50c32c148cb64e8f1981928afd84eef382420271f9eea03`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 5.0 KB (5036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c92c233bf14760a22129e5c30a446df97f50b059c4f0b9c2dae8c921ffd9e7`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.28-focal`

```console
$ docker pull mariadb@sha256:df7edb9de3ba069b6d5dfc4882798d11b401817a0d166d0f6076eb9865313920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.28-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:b5a051d8feaa86aed3d62b55d8ff5b457bb4754b5e7ba21e63d9ca4ccb3f5af7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118327915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512186ae7f53662017f42a73f8dd5ce822aacd9873b847f28a8ccf20868f4293`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:33:25 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 24 Apr 2021 00:33:25 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 24 Apr 2021 00:33:26 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:33:53 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:33:54 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:33:54 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:33:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:33:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:33:55 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:33:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7fc27a6a863a4620fc3da7c2aa4c8b4b2ee5fcca88f459cf0fedbdcd548fd4`  
		Last Modified: Sat, 24 Apr 2021 00:37:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04e45a90e173ff1f3ccfc630bea9526918dd0dc5a74a011819679fa0e29c885`  
		Last Modified: Sat, 24 Apr 2021 00:38:06 GMT  
		Size: 81.7 MB (81687842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc20c2d0927609ab8ac205f7f27cfc8194bf7993dbf2f9595e850862bc516250`  
		Last Modified: Sat, 24 Apr 2021 00:37:52 GMT  
		Size: 5.0 KB (5028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e189f24a7dd6b6739c7a6110ba3fe8065f5208974dc4386cfed6426fef855b`  
		Last Modified: Sat, 24 Apr 2021 00:37:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:4bd68304b338c591eb5aa39033826107013f44960d859a5f48d6268c0a605b52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116006894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1887b121bf3b90fbcc249a1ebff3282f415a5f06c84eff80c0024c541bf4cbc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:36:34 GMT
ENV MARIADB_MAJOR=10.3
# Fri, 23 Apr 2021 23:36:35 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Fri, 23 Apr 2021 23:36:41 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:37:29 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:37:31 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:37:32 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:37:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:37:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:37:36 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:37:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be52582cab73354a0e4d897c88d485858f8fa1dc98ec8e982faeb9dba19d9c2f`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8173267e77964d10ccb5049b81b0f4385e0af4e269c76841c0eba9080b813b`  
		Last Modified: Fri, 23 Apr 2021 23:44:06 GMT  
		Size: 80.9 MB (80862291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff99a2d812b02ad30fe65d4d74e60806e891cddc13ca8714feec8d6d8567df6`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971b6f235d6345df394933f34c380b68e8ebb0e6487f49246d3c45a1de3f04a9`  
		Last Modified: Fri, 23 Apr 2021 23:43:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:3dadd2ddf07aaa2418e09f614561c5b8151f081747de9c07b5b3cefd14cd18bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128898109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bc4cbb89eff87d0cb24e3c59a939e80ab6cf07bdd38129a70bda6b677385cef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 02:00:08 GMT
ENV MARIADB_MAJOR=10.3
# Sat, 24 Apr 2021 02:00:12 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Sat, 24 Apr 2021 02:00:25 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 02:02:51 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 02:03:02 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 02:03:04 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 02:03:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 02:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 02:03:15 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 02:03:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd5d0d35665f927618341beedb67deb8837c42b6e358619057b9ca430db0d8e`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f89cd035af5eb9af324668b04fe04636f7ad396708f2d6dd431db2a853c53f9`  
		Last Modified: Sat, 24 Apr 2021 02:18:00 GMT  
		Size: 86.4 MB (86437537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f265070eaaf750af50c32c148cb64e8f1981928afd84eef382420271f9eea03`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 5.0 KB (5036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c92c233bf14760a22129e5c30a446df97f50b059c4f0b9c2dae8c921ffd9e7`  
		Last Modified: Sat, 24 Apr 2021 02:17:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:b4b1eb5307871017c62704bc58e893b7fb3706248fd3aca0f37063f53f42617e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:d193d9c74777e74d77b6d903a6f5cc0548e50ae7ccd42c1c152ae623c42ada8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122200358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37406e27ca2ca5b595b59326ff05b2626f2b8d287b1d7ab4f83dd648e5b2d0fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:59 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 24 Apr 2021 00:32:59 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 24 Apr 2021 00:33:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:33:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:33:20 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:33:20 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:33:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:33:22 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:33:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262af926fc4b7c85cf156639b1e1fe9e601c6498b459a6d164dd2331532c912d`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698769d7042b5aceaad99808e9f8fd1cf0275f1a73560b9d4fc461177fb96b0e`  
		Last Modified: Sat, 24 Apr 2021 00:37:34 GMT  
		Size: 85.6 MB (85560280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d50f861d6e81dad7ec16af83d8a98ba8057f589103c59e75b4aa28b8bd01ab`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4a67dee109e7a8dd059591252e15769edb1cd5cd81d215d3d69ed5a64920b7`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:528987f0a5c2029363a3f414274fde043c971cc93c0dfceb736b47d437f9d59d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119775878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5adcf31720a6aacd1165884f3df0416cbecf10567e0b48a1af08e5e5db84a6df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:35:15 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 23 Apr 2021 23:35:16 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Fri, 23 Apr 2021 23:35:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:36:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:36:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:36:07 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:36:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:36:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:36:14 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5f7bc3a83d0b867b07b5c9acb951cce5c9d9b228348996e4a8bc651340e4b6`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b08ae5280f18140db774effa7b365a18acc25b027b4aee0d332e4c377cbba6`  
		Last Modified: Fri, 23 Apr 2021 23:43:23 GMT  
		Size: 84.6 MB (84631273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae84ea1e99108e53729dd900ecf56d46810519a2dd5a3ce37bc273d8004a99`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d93f56208eb9d2b8485bdc3ba48d208f5e71f6a9b32e2f17e1e0cb743acdbca`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d0738ed703cd2a987d490eb4e3d990e6c83add103356ca25767335f56d9de415
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132578026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d7ff893aa534dff15282c4b09f67645100dc3cb09356ea42af92f7382966e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:56:42 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 24 Apr 2021 01:56:45 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 24 Apr 2021 01:56:51 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:59:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:59:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:59:37 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:59:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 01:59:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:59:50 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:59:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3671bb3366525ca64a9a14a0853aa8b418e2feee50f57d7eb89ea132819268b6`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93028cecaf1e27ddaa2117ad15e243764781b9a4882da1f3e3f50cc8694a6ee8`  
		Last Modified: Sat, 24 Apr 2021 02:17:25 GMT  
		Size: 90.1 MB (90117458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d208c6932ddf65d10d9a75383fc57c36ddbebd5148346675d64d5f3333bec6`  
		Last Modified: Sat, 24 Apr 2021 02:17:02 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3814e80a8ecd1f02675621e5b0c85f0c917499c5ce95632239de58d593a7b6d9`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:b4b1eb5307871017c62704bc58e893b7fb3706248fd3aca0f37063f53f42617e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d193d9c74777e74d77b6d903a6f5cc0548e50ae7ccd42c1c152ae623c42ada8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122200358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37406e27ca2ca5b595b59326ff05b2626f2b8d287b1d7ab4f83dd648e5b2d0fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:59 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 24 Apr 2021 00:32:59 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 24 Apr 2021 00:33:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:33:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:33:20 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:33:20 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:33:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:33:22 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:33:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262af926fc4b7c85cf156639b1e1fe9e601c6498b459a6d164dd2331532c912d`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698769d7042b5aceaad99808e9f8fd1cf0275f1a73560b9d4fc461177fb96b0e`  
		Last Modified: Sat, 24 Apr 2021 00:37:34 GMT  
		Size: 85.6 MB (85560280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d50f861d6e81dad7ec16af83d8a98ba8057f589103c59e75b4aa28b8bd01ab`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4a67dee109e7a8dd059591252e15769edb1cd5cd81d215d3d69ed5a64920b7`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:528987f0a5c2029363a3f414274fde043c971cc93c0dfceb736b47d437f9d59d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119775878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5adcf31720a6aacd1165884f3df0416cbecf10567e0b48a1af08e5e5db84a6df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:35:15 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 23 Apr 2021 23:35:16 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Fri, 23 Apr 2021 23:35:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:36:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:36:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:36:07 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:36:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:36:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:36:14 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5f7bc3a83d0b867b07b5c9acb951cce5c9d9b228348996e4a8bc651340e4b6`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b08ae5280f18140db774effa7b365a18acc25b027b4aee0d332e4c377cbba6`  
		Last Modified: Fri, 23 Apr 2021 23:43:23 GMT  
		Size: 84.6 MB (84631273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae84ea1e99108e53729dd900ecf56d46810519a2dd5a3ce37bc273d8004a99`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d93f56208eb9d2b8485bdc3ba48d208f5e71f6a9b32e2f17e1e0cb743acdbca`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d0738ed703cd2a987d490eb4e3d990e6c83add103356ca25767335f56d9de415
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132578026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d7ff893aa534dff15282c4b09f67645100dc3cb09356ea42af92f7382966e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:56:42 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 24 Apr 2021 01:56:45 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 24 Apr 2021 01:56:51 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:59:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:59:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:59:37 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:59:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 01:59:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:59:50 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:59:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3671bb3366525ca64a9a14a0853aa8b418e2feee50f57d7eb89ea132819268b6`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93028cecaf1e27ddaa2117ad15e243764781b9a4882da1f3e3f50cc8694a6ee8`  
		Last Modified: Sat, 24 Apr 2021 02:17:25 GMT  
		Size: 90.1 MB (90117458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d208c6932ddf65d10d9a75383fc57c36ddbebd5148346675d64d5f3333bec6`  
		Last Modified: Sat, 24 Apr 2021 02:17:02 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3814e80a8ecd1f02675621e5b0c85f0c917499c5ce95632239de58d593a7b6d9`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.18`

```console
$ docker pull mariadb@sha256:b4b1eb5307871017c62704bc58e893b7fb3706248fd3aca0f37063f53f42617e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.18` - linux; amd64

```console
$ docker pull mariadb@sha256:d193d9c74777e74d77b6d903a6f5cc0548e50ae7ccd42c1c152ae623c42ada8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122200358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37406e27ca2ca5b595b59326ff05b2626f2b8d287b1d7ab4f83dd648e5b2d0fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:59 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 24 Apr 2021 00:32:59 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 24 Apr 2021 00:33:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:33:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:33:20 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:33:20 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:33:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:33:22 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:33:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262af926fc4b7c85cf156639b1e1fe9e601c6498b459a6d164dd2331532c912d`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698769d7042b5aceaad99808e9f8fd1cf0275f1a73560b9d4fc461177fb96b0e`  
		Last Modified: Sat, 24 Apr 2021 00:37:34 GMT  
		Size: 85.6 MB (85560280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d50f861d6e81dad7ec16af83d8a98ba8057f589103c59e75b4aa28b8bd01ab`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4a67dee109e7a8dd059591252e15769edb1cd5cd81d215d3d69ed5a64920b7`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:528987f0a5c2029363a3f414274fde043c971cc93c0dfceb736b47d437f9d59d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119775878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5adcf31720a6aacd1165884f3df0416cbecf10567e0b48a1af08e5e5db84a6df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:35:15 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 23 Apr 2021 23:35:16 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Fri, 23 Apr 2021 23:35:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:36:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:36:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:36:07 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:36:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:36:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:36:14 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5f7bc3a83d0b867b07b5c9acb951cce5c9d9b228348996e4a8bc651340e4b6`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b08ae5280f18140db774effa7b365a18acc25b027b4aee0d332e4c377cbba6`  
		Last Modified: Fri, 23 Apr 2021 23:43:23 GMT  
		Size: 84.6 MB (84631273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae84ea1e99108e53729dd900ecf56d46810519a2dd5a3ce37bc273d8004a99`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d93f56208eb9d2b8485bdc3ba48d208f5e71f6a9b32e2f17e1e0cb743acdbca`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d0738ed703cd2a987d490eb4e3d990e6c83add103356ca25767335f56d9de415
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132578026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d7ff893aa534dff15282c4b09f67645100dc3cb09356ea42af92f7382966e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:56:42 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 24 Apr 2021 01:56:45 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 24 Apr 2021 01:56:51 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:59:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:59:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:59:37 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:59:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 01:59:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:59:50 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:59:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3671bb3366525ca64a9a14a0853aa8b418e2feee50f57d7eb89ea132819268b6`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93028cecaf1e27ddaa2117ad15e243764781b9a4882da1f3e3f50cc8694a6ee8`  
		Last Modified: Sat, 24 Apr 2021 02:17:25 GMT  
		Size: 90.1 MB (90117458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d208c6932ddf65d10d9a75383fc57c36ddbebd5148346675d64d5f3333bec6`  
		Last Modified: Sat, 24 Apr 2021 02:17:02 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3814e80a8ecd1f02675621e5b0c85f0c917499c5ce95632239de58d593a7b6d9`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.18-focal`

```console
$ docker pull mariadb@sha256:b4b1eb5307871017c62704bc58e893b7fb3706248fd3aca0f37063f53f42617e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.18-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d193d9c74777e74d77b6d903a6f5cc0548e50ae7ccd42c1c152ae623c42ada8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122200358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37406e27ca2ca5b595b59326ff05b2626f2b8d287b1d7ab4f83dd648e5b2d0fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:59 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 24 Apr 2021 00:32:59 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 24 Apr 2021 00:33:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:33:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:33:20 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:33:20 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:33:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 00:33:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:33:22 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:33:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262af926fc4b7c85cf156639b1e1fe9e601c6498b459a6d164dd2331532c912d`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698769d7042b5aceaad99808e9f8fd1cf0275f1a73560b9d4fc461177fb96b0e`  
		Last Modified: Sat, 24 Apr 2021 00:37:34 GMT  
		Size: 85.6 MB (85560280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d50f861d6e81dad7ec16af83d8a98ba8057f589103c59e75b4aa28b8bd01ab`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4a67dee109e7a8dd059591252e15769edb1cd5cd81d215d3d69ed5a64920b7`  
		Last Modified: Sat, 24 Apr 2021 00:37:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:528987f0a5c2029363a3f414274fde043c971cc93c0dfceb736b47d437f9d59d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119775878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5adcf31720a6aacd1165884f3df0416cbecf10567e0b48a1af08e5e5db84a6df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:35:15 GMT
ENV MARIADB_MAJOR=10.4
# Fri, 23 Apr 2021 23:35:16 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Fri, 23 Apr 2021 23:35:19 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:36:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:36:05 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:36:07 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:36:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 23:36:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:36:14 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:36:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5f7bc3a83d0b867b07b5c9acb951cce5c9d9b228348996e4a8bc651340e4b6`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b08ae5280f18140db774effa7b365a18acc25b027b4aee0d332e4c377cbba6`  
		Last Modified: Fri, 23 Apr 2021 23:43:23 GMT  
		Size: 84.6 MB (84631273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae84ea1e99108e53729dd900ecf56d46810519a2dd5a3ce37bc273d8004a99`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d93f56208eb9d2b8485bdc3ba48d208f5e71f6a9b32e2f17e1e0cb743acdbca`  
		Last Modified: Fri, 23 Apr 2021 23:42:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:d0738ed703cd2a987d490eb4e3d990e6c83add103356ca25767335f56d9de415
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132578026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74d7ff893aa534dff15282c4b09f67645100dc3cb09356ea42af92f7382966e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:56:42 GMT
ENV MARIADB_MAJOR=10.4
# Sat, 24 Apr 2021 01:56:45 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Sat, 24 Apr 2021 01:56:51 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:59:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:59:32 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:59:37 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:59:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 24 Apr 2021 01:59:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:59:50 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:59:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3671bb3366525ca64a9a14a0853aa8b418e2feee50f57d7eb89ea132819268b6`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93028cecaf1e27ddaa2117ad15e243764781b9a4882da1f3e3f50cc8694a6ee8`  
		Last Modified: Sat, 24 Apr 2021 02:17:25 GMT  
		Size: 90.1 MB (90117458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d208c6932ddf65d10d9a75383fc57c36ddbebd5148346675d64d5f3333bec6`  
		Last Modified: Sat, 24 Apr 2021 02:17:02 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3814e80a8ecd1f02675621e5b0c85f0c917499c5ce95632239de58d593a7b6d9`  
		Last Modified: Sat, 24 Apr 2021 02:17:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:36288c675a192bd0a8a99cd6ba0780e31df85f0bfd0cbb204837cd108be3d236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:a362c0e1cffc6530e43e96e8bdd73d5735f3b5a7f4e1ae04667cf7285ca1ee1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124217165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992bce5ed7107642a27af59c2a2ddb7e589a44b639342b9501044511ab00aca0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 00:32:14 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:32:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:32:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:32:45 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:32:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:32:46 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:32:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a5dea1514db115cf28f9794262ca153c674751a11a39302a0ce3db6256c1d0`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5cf124c10ff33f1c7248e77e4ecaf76c89f19cdd826302c8ef54f2ac483ba`  
		Last Modified: Sat, 24 Apr 2021 00:36:47 GMT  
		Size: 87.6 MB (87577210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3352c2c9d21ce50c5af85c0fd16ddbed1a456eee52a5a34f44b465b7ff406281`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b01b1f9f4e04d4946c955b3e11a874f26791ca60cd305bda9999e43ca68be88c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121798059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9897eef8d73ac349375648c162a7b658565ed9a1a1dd36b6983adb19adccd5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:33:56 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 23 Apr 2021 23:33:57 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Fri, 23 Apr 2021 23:34:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:34:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:34:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:34:50 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:34:53 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:34:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf92de28cc1b694eb83365182205da153a31159d5d9ab06c67985100bd667ab`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb658d2a8224cd4532d094e05764d42def5d4974b2078d085c7c0d93a2d9056`  
		Last Modified: Fri, 23 Apr 2021 23:42:35 GMT  
		Size: 86.7 MB (86653573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34a83a38d8cdd7a6fe7f1ff714a32d6d452fab5f0bb34975b43ef2ceb99117`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:631c39535cd04a4614f510eb08d6a38edaa6155f1a793b0e6aee22249e6dfdd9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134658895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96625041fe6e55357b7eab093c0b90593fb9ef59c59bfc73b646ed4fb7a302de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:33 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 01:53:37 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 01:53:45 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:56:08 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:56:16 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:56:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:56:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:56:23 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3623b2360b0968a252476fb127f16f81174b3b9177234d78a4438374e6ff647`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58fb477779bd9749213f204c72c054541a404357cdc24fd2555478c8085c0b`  
		Last Modified: Sat, 24 Apr 2021 02:16:33 GMT  
		Size: 92.2 MB (92198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab7f51766b107f9d8e24502ceb64428358ff7c94d2742019b69259962d5f41`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:36288c675a192bd0a8a99cd6ba0780e31df85f0bfd0cbb204837cd108be3d236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a362c0e1cffc6530e43e96e8bdd73d5735f3b5a7f4e1ae04667cf7285ca1ee1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124217165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992bce5ed7107642a27af59c2a2ddb7e589a44b639342b9501044511ab00aca0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 00:32:14 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:32:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:32:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:32:45 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:32:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:32:46 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:32:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a5dea1514db115cf28f9794262ca153c674751a11a39302a0ce3db6256c1d0`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5cf124c10ff33f1c7248e77e4ecaf76c89f19cdd826302c8ef54f2ac483ba`  
		Last Modified: Sat, 24 Apr 2021 00:36:47 GMT  
		Size: 87.6 MB (87577210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3352c2c9d21ce50c5af85c0fd16ddbed1a456eee52a5a34f44b465b7ff406281`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b01b1f9f4e04d4946c955b3e11a874f26791ca60cd305bda9999e43ca68be88c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121798059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9897eef8d73ac349375648c162a7b658565ed9a1a1dd36b6983adb19adccd5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:33:56 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 23 Apr 2021 23:33:57 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Fri, 23 Apr 2021 23:34:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:34:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:34:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:34:50 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:34:53 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:34:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf92de28cc1b694eb83365182205da153a31159d5d9ab06c67985100bd667ab`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb658d2a8224cd4532d094e05764d42def5d4974b2078d085c7c0d93a2d9056`  
		Last Modified: Fri, 23 Apr 2021 23:42:35 GMT  
		Size: 86.7 MB (86653573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34a83a38d8cdd7a6fe7f1ff714a32d6d452fab5f0bb34975b43ef2ceb99117`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:631c39535cd04a4614f510eb08d6a38edaa6155f1a793b0e6aee22249e6dfdd9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134658895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96625041fe6e55357b7eab093c0b90593fb9ef59c59bfc73b646ed4fb7a302de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:33 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 01:53:37 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 01:53:45 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:56:08 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:56:16 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:56:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:56:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:56:23 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3623b2360b0968a252476fb127f16f81174b3b9177234d78a4438374e6ff647`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58fb477779bd9749213f204c72c054541a404357cdc24fd2555478c8085c0b`  
		Last Modified: Sat, 24 Apr 2021 02:16:33 GMT  
		Size: 92.2 MB (92198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab7f51766b107f9d8e24502ceb64428358ff7c94d2742019b69259962d5f41`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.9`

```console
$ docker pull mariadb@sha256:36288c675a192bd0a8a99cd6ba0780e31df85f0bfd0cbb204837cd108be3d236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.9` - linux; amd64

```console
$ docker pull mariadb@sha256:a362c0e1cffc6530e43e96e8bdd73d5735f3b5a7f4e1ae04667cf7285ca1ee1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124217165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992bce5ed7107642a27af59c2a2ddb7e589a44b639342b9501044511ab00aca0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 00:32:14 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:32:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:32:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:32:45 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:32:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:32:46 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:32:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a5dea1514db115cf28f9794262ca153c674751a11a39302a0ce3db6256c1d0`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5cf124c10ff33f1c7248e77e4ecaf76c89f19cdd826302c8ef54f2ac483ba`  
		Last Modified: Sat, 24 Apr 2021 00:36:47 GMT  
		Size: 87.6 MB (87577210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3352c2c9d21ce50c5af85c0fd16ddbed1a456eee52a5a34f44b465b7ff406281`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b01b1f9f4e04d4946c955b3e11a874f26791ca60cd305bda9999e43ca68be88c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121798059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9897eef8d73ac349375648c162a7b658565ed9a1a1dd36b6983adb19adccd5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:33:56 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 23 Apr 2021 23:33:57 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Fri, 23 Apr 2021 23:34:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:34:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:34:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:34:50 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:34:53 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:34:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf92de28cc1b694eb83365182205da153a31159d5d9ab06c67985100bd667ab`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb658d2a8224cd4532d094e05764d42def5d4974b2078d085c7c0d93a2d9056`  
		Last Modified: Fri, 23 Apr 2021 23:42:35 GMT  
		Size: 86.7 MB (86653573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34a83a38d8cdd7a6fe7f1ff714a32d6d452fab5f0bb34975b43ef2ceb99117`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9` - linux; ppc64le

```console
$ docker pull mariadb@sha256:631c39535cd04a4614f510eb08d6a38edaa6155f1a793b0e6aee22249e6dfdd9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134658895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96625041fe6e55357b7eab093c0b90593fb9ef59c59bfc73b646ed4fb7a302de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:33 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 01:53:37 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 01:53:45 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:56:08 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:56:16 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:56:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:56:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:56:23 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3623b2360b0968a252476fb127f16f81174b3b9177234d78a4438374e6ff647`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58fb477779bd9749213f204c72c054541a404357cdc24fd2555478c8085c0b`  
		Last Modified: Sat, 24 Apr 2021 02:16:33 GMT  
		Size: 92.2 MB (92198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab7f51766b107f9d8e24502ceb64428358ff7c94d2742019b69259962d5f41`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.9-focal`

```console
$ docker pull mariadb@sha256:36288c675a192bd0a8a99cd6ba0780e31df85f0bfd0cbb204837cd108be3d236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.9-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a362c0e1cffc6530e43e96e8bdd73d5735f3b5a7f4e1ae04667cf7285ca1ee1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124217165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992bce5ed7107642a27af59c2a2ddb7e589a44b639342b9501044511ab00aca0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 00:32:14 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:32:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:32:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:32:45 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:32:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:32:46 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:32:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a5dea1514db115cf28f9794262ca153c674751a11a39302a0ce3db6256c1d0`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5cf124c10ff33f1c7248e77e4ecaf76c89f19cdd826302c8ef54f2ac483ba`  
		Last Modified: Sat, 24 Apr 2021 00:36:47 GMT  
		Size: 87.6 MB (87577210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3352c2c9d21ce50c5af85c0fd16ddbed1a456eee52a5a34f44b465b7ff406281`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b01b1f9f4e04d4946c955b3e11a874f26791ca60cd305bda9999e43ca68be88c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121798059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9897eef8d73ac349375648c162a7b658565ed9a1a1dd36b6983adb19adccd5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:33:56 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 23 Apr 2021 23:33:57 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Fri, 23 Apr 2021 23:34:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:34:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:34:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:34:50 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:34:53 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:34:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf92de28cc1b694eb83365182205da153a31159d5d9ab06c67985100bd667ab`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb658d2a8224cd4532d094e05764d42def5d4974b2078d085c7c0d93a2d9056`  
		Last Modified: Fri, 23 Apr 2021 23:42:35 GMT  
		Size: 86.7 MB (86653573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34a83a38d8cdd7a6fe7f1ff714a32d6d452fab5f0bb34975b43ef2ceb99117`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:631c39535cd04a4614f510eb08d6a38edaa6155f1a793b0e6aee22249e6dfdd9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134658895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96625041fe6e55357b7eab093c0b90593fb9ef59c59bfc73b646ed4fb7a302de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:33 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 01:53:37 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 01:53:45 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:56:08 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:56:16 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:56:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:56:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:56:23 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3623b2360b0968a252476fb127f16f81174b3b9177234d78a4438374e6ff647`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58fb477779bd9749213f204c72c054541a404357cdc24fd2555478c8085c0b`  
		Last Modified: Sat, 24 Apr 2021 02:16:33 GMT  
		Size: 92.2 MB (92198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab7f51766b107f9d8e24502ceb64428358ff7c94d2742019b69259962d5f41`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:36288c675a192bd0a8a99cd6ba0780e31df85f0bfd0cbb204837cd108be3d236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:a362c0e1cffc6530e43e96e8bdd73d5735f3b5a7f4e1ae04667cf7285ca1ee1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124217165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992bce5ed7107642a27af59c2a2ddb7e589a44b639342b9501044511ab00aca0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 00:32:14 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:32:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:32:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:32:45 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:32:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:32:46 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:32:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a5dea1514db115cf28f9794262ca153c674751a11a39302a0ce3db6256c1d0`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5cf124c10ff33f1c7248e77e4ecaf76c89f19cdd826302c8ef54f2ac483ba`  
		Last Modified: Sat, 24 Apr 2021 00:36:47 GMT  
		Size: 87.6 MB (87577210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3352c2c9d21ce50c5af85c0fd16ddbed1a456eee52a5a34f44b465b7ff406281`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b01b1f9f4e04d4946c955b3e11a874f26791ca60cd305bda9999e43ca68be88c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121798059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9897eef8d73ac349375648c162a7b658565ed9a1a1dd36b6983adb19adccd5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:33:56 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 23 Apr 2021 23:33:57 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Fri, 23 Apr 2021 23:34:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:34:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:34:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:34:50 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:34:53 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:34:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf92de28cc1b694eb83365182205da153a31159d5d9ab06c67985100bd667ab`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb658d2a8224cd4532d094e05764d42def5d4974b2078d085c7c0d93a2d9056`  
		Last Modified: Fri, 23 Apr 2021 23:42:35 GMT  
		Size: 86.7 MB (86653573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34a83a38d8cdd7a6fe7f1ff714a32d6d452fab5f0bb34975b43ef2ceb99117`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:631c39535cd04a4614f510eb08d6a38edaa6155f1a793b0e6aee22249e6dfdd9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134658895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96625041fe6e55357b7eab093c0b90593fb9ef59c59bfc73b646ed4fb7a302de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:33 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 01:53:37 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 01:53:45 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:56:08 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:56:16 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:56:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:56:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:56:23 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3623b2360b0968a252476fb127f16f81174b3b9177234d78a4438374e6ff647`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58fb477779bd9749213f204c72c054541a404357cdc24fd2555478c8085c0b`  
		Last Modified: Sat, 24 Apr 2021 02:16:33 GMT  
		Size: 92.2 MB (92198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab7f51766b107f9d8e24502ceb64428358ff7c94d2742019b69259962d5f41`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:36288c675a192bd0a8a99cd6ba0780e31df85f0bfd0cbb204837cd108be3d236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:a362c0e1cffc6530e43e96e8bdd73d5735f3b5a7f4e1ae04667cf7285ca1ee1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124217165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992bce5ed7107642a27af59c2a2ddb7e589a44b639342b9501044511ab00aca0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 00:31:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 00:31:55 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:31:55 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 00:32:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 00:32:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 00:32:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 00:32:12 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 00:32:13 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 00:32:13 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 00:32:14 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 00:32:44 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 00:32:45 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 00:32:45 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 00:32:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 00:32:46 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 00:32:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d512e2ff7788e9e77850c0a2830d054527a099b682ed31eadb5331161f96559`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c1a7dc2af94808125e8bd4d5ddfe0d556ff280e6897a9cef8276e1f6225f20`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 5.5 MB (5490249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1da40ab8a23e6094782efb78962eb99f7522ad555cd15b55d8cbab37ac0ece`  
		Last Modified: Sat, 24 Apr 2021 00:36:37 GMT  
		Size: 1.3 MB (1326250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5cfc6687263b6f32a11c0f9db8df79668f42d8d46a0379faba2a3a6489ed72`  
		Last Modified: Sat, 24 Apr 2021 00:36:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb86f2976144f88f6d41e8e5dbcbe5e12bb50a34e2747447c058a9ce3b4f2a6`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 1.3 MB (1273046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861f77e80d57cbd5666826845514ffc10733e3000a1592981d6a0c3574c3b95`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a5dea1514db115cf28f9794262ca153c674751a11a39302a0ce3db6256c1d0`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b5cf124c10ff33f1c7248e77e4ecaf76c89f19cdd826302c8ef54f2ac483ba`  
		Last Modified: Sat, 24 Apr 2021 00:36:47 GMT  
		Size: 87.6 MB (87577210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3352c2c9d21ce50c5af85c0fd16ddbed1a456eee52a5a34f44b465b7ff406281`  
		Last Modified: Sat, 24 Apr 2021 00:36:33 GMT  
		Size: 5.0 KB (5029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:b01b1f9f4e04d4946c955b3e11a874f26791ca60cd305bda9999e43ca68be88c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121798059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9897eef8d73ac349375648c162a7b658565ed9a1a1dd36b6983adb19adccd5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:47:51 GMT
ADD file:57e6f432b1329c286e596ded8065bebdfc70a87fae91dd79bd805363ef008e5d in / 
# Fri, 23 Apr 2021 22:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:47:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:47:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:47:59 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:32:57 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Apr 2021 23:33:15 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:17 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Apr 2021 23:33:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Apr 2021 23:33:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Apr 2021 23:33:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 23:33:52 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Apr 2021 23:33:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Apr 2021 23:33:56 GMT
ENV MARIADB_MAJOR=10.5
# Fri, 23 Apr 2021 23:33:57 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Fri, 23 Apr 2021 23:34:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 23 Apr 2021 23:34:45 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Fri, 23 Apr 2021 23:34:49 GMT
VOLUME [/var/lib/mysql]
# Fri, 23 Apr 2021 23:34:50 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Fri, 23 Apr 2021 23:34:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 23:34:53 GMT
EXPOSE 3306
# Fri, 23 Apr 2021 23:34:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:80bc30679ac1fd798f3241208c14accd6a364cb8a6224d1127dfb1577d10554f`  
		Last Modified: Fri, 16 Apr 2021 08:25:26 GMT  
		Size: 27.1 MB (27144417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf18fab4cfbf479fa9f8409ad47e2702c63241304c2cdd4c33f2a1633c5f85e`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979309c983a2adeff352538937475cf961d49c34194fa2aab142effe19ed9c1`  
		Last Modified: Fri, 23 Apr 2021 22:50:04 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4d4c2f8c52ab8718b164e63d5660a1f3855bc8691a1af295eef9fa7ffb9ed`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98569ed213826fdb6495541f24382e56a5640b8ebe3a52c578a3c0e7e59512af`  
		Last Modified: Fri, 23 Apr 2021 23:42:18 GMT  
		Size: 5.5 MB (5455728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928b768e6825f5a29f903eed57c97bf4497cc01e241e05d7b1ee32b3a7ccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:17 GMT  
		Size: 1.3 MB (1262314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b262239453e8f4675a80bd13c1d8a8f9d62c89afb7373c8c8a6343d3cc9a1`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd1d632c443f7fdeb198a105f5a3b6f2e38f49e5a0bf5e5363d9ace6842b9e5`  
		Last Modified: Fri, 23 Apr 2021 23:42:15 GMT  
		Size: 1.3 MB (1271226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dfea8d78f69e414c6d55419ea0ccc8d7bdd0faa5add9a051fdb7c9af8fcccb`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf92de28cc1b694eb83365182205da153a31159d5d9ab06c67985100bd667ab`  
		Last Modified: Fri, 23 Apr 2021 23:42:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb658d2a8224cd4532d094e05764d42def5d4974b2078d085c7c0d93a2d9056`  
		Last Modified: Fri, 23 Apr 2021 23:42:35 GMT  
		Size: 86.7 MB (86653573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34a83a38d8cdd7a6fe7f1ff714a32d6d452fab5f0bb34975b43ef2ceb99117`  
		Last Modified: Fri, 23 Apr 2021 23:42:14 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:631c39535cd04a4614f510eb08d6a38edaa6155f1a793b0e6aee22249e6dfdd9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134658895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96625041fe6e55357b7eab093c0b90593fb9ef59c59bfc73b646ed4fb7a302de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:50:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 24 Apr 2021 01:51:59 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:52:04 GMT
ENV GOSU_VERSION=1.12
# Sat, 24 Apr 2021 01:52:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 24 Apr 2021 01:52:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 24 Apr 2021 01:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:53:23 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 24 Apr 2021 01:53:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 24 Apr 2021 01:53:33 GMT
ENV MARIADB_MAJOR=10.5
# Sat, 24 Apr 2021 01:53:37 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Sat, 24 Apr 2021 01:53:45 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Sat, 24 Apr 2021 01:56:08 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Sat, 24 Apr 2021 01:56:16 GMT
VOLUME [/var/lib/mysql]
# Sat, 24 Apr 2021 01:56:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Sat, 24 Apr 2021 01:56:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Apr 2021 01:56:23 GMT
EXPOSE 3306
# Sat, 24 Apr 2021 01:56:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d305ff3127f29761eb61cc5752ae35b85fd17887d052bca1af891821908bf`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a124c3f9fa2a98515fcfb8511b8ca6ae72304bb9d12506f7a0293357b7761e`  
		Last Modified: Sat, 24 Apr 2021 02:16:19 GMT  
		Size: 6.7 MB (6668282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6aec671cb5af515276c6ab060c662264540289f47965b6f1ed5990e2b9857a8`  
		Last Modified: Sat, 24 Apr 2021 02:16:16 GMT  
		Size: 1.2 MB (1244728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9a34e20437321fa36a02e623306a5ae3a70e18dc62fcd831182874dc5cf776`  
		Last Modified: Sat, 24 Apr 2021 02:16:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badea69f99ac94b3d9e60fae29e367d9adc4499ee6564a50f519e9971afa9a6b`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 1.3 MB (1281250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b719541110114f61faa22db2ead41ac79f3ccfd3417c1d7aa6cd5d2d4815e`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3623b2360b0968a252476fb127f16f81174b3b9177234d78a4438374e6ff647`  
		Last Modified: Sat, 24 Apr 2021 02:16:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58fb477779bd9749213f204c72c054541a404357cdc24fd2555478c8085c0b`  
		Last Modified: Sat, 24 Apr 2021 02:16:33 GMT  
		Size: 92.2 MB (92198447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab7f51766b107f9d8e24502ceb64428358ff7c94d2742019b69259962d5f41`  
		Last Modified: Sat, 24 Apr 2021 02:16:12 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
