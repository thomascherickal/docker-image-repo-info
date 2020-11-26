<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10.1`](#mariadb101)
-	[`mariadb:10.1.48`](#mariadb10148)
-	[`mariadb:10.1.48-bionic`](#mariadb10148-bionic)
-	[`mariadb:10.1-bionic`](#mariadb101-bionic)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2.36`](#mariadb10236)
-	[`mariadb:10.2.36-bionic`](#mariadb10236-bionic)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3.27`](#mariadb10327)
-	[`mariadb:10.3.27-focal`](#mariadb10327-focal)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4.17`](#mariadb10417)
-	[`mariadb:10.4.17-focal`](#mariadb10417-focal)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5.8`](#mariadb1058)
-	[`mariadb:10.5.8-focal`](#mariadb1058-focal)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:a497d4046a9762617f3203c3c42ab06c78f7e4a2663fed9b3e7f205da7b02d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:be0069ebc09c00f5ff0b1900c5df05eb201cc01d3df4ab7828d26d38fae81654
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125585067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a348a04a8159339ed3ca053ea925f854252e6a6c3df6fa82c17625d1026f18b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 25 Nov 2020 23:18:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:18:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:18:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:18:41 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:18:41 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:18:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8690a3260b734a0e2fe29912f283112edfc4aa22a31bf7282282726e993a8cc`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202ba90333a4d33b3cdeeefcac43e219ea015f484b4b92e14f865621128e237`  
		Last Modified: Wed, 25 Nov 2020 23:22:42 GMT  
		Size: 88.9 MB (88930464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f860b4aa6bf9c5c6f3949001e39c976ac2eddf08295ab842bdc34114ac910`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2b3ef213bead7e743f8b4b3b6fa921cbc963b50a0e89629d934d36c5f2cf7db3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125341391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb59cafebcdf0d75c35d5f018b2192f12e489322be0d89f2ad2bad29635950f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:34:48 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:40:12 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:40:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:41:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:41:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:41:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:41:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:41:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4043d13620ba09e5adff91c927c808500013ef40718f9c667fc415edbbb0fc14`  
		Last Modified: Wed, 11 Nov 2020 21:45:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18247d5d96cbb0445be3ca7366b78e3898db90f269e221dc6a352dd26913431`  
		Last Modified: Wed, 11 Nov 2020 21:46:08 GMT  
		Size: 90.2 MB (90183417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189428954a19e532b3b3af8a3e672fc6513780d0adf3d36d9e5f00228dc2ee94`  
		Last Modified: Wed, 11 Nov 2020 21:45:45 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a9703d1360fae84a4ff8df8d073465ddf5c2f5f12bb4aebd813a5cde3237fed7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137899523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87db369b2668d9ef78329de8a3058dec7d07735661d3489ee8caae0906a89275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:02:43 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:18:26 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:18:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:24:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:24:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:24:27 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988eb6532774207788d05dbdf4b3d057780e0ef2fa395bb5badad4085831dba`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b92a77676842ce52974bfdc0b071724e52629f89ece0aea76241e73e5b846d`  
		Last Modified: Wed, 11 Nov 2020 21:49:43 GMT  
		Size: 95.4 MB (95426507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1080dd4f32be8bc637c4fe10ddef90f2dba8cc8466e816c6263e10af214e06e`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1`

```console
$ docker pull mariadb@sha256:c1b13e294590066f390710d63f64324d5a42f5e0ba7680816f642e32727ee6f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1` - linux; amd64

```console
$ docker pull mariadb@sha256:aa5b677a55dae30f6c7694a63b92fb53988a8a241df09f7dc48bf8016c8f8388
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113172303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d374fe48b4e1d02456b69dfca8c49c4c6b70ef6565625813ba3ecae29c4ddc86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:20:10 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:20:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:20:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:20:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:20:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:21:26 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 25 Nov 2020 23:21:26 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 25 Nov 2020 23:21:27 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:22:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:22:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:22:02 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:22:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:22:04 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:22:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12260b0e97bc71b9bff6cd1af9e1c9c8bddccbc0e8c8198a4d49fc8bcec162e3`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a55695dfa04b41d261954f037febf6e4541519bd02fe4bdb1e48a0a7c4b31`  
		Last Modified: Wed, 25 Nov 2020 23:23:46 GMT  
		Size: 4.8 MB (4811249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b965e29cfef068223e351c81acb95c2305cf13e74ce8c12d82b7f4bfcc5042e`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 1.3 MB (1326975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013e2bd9bdd9019386d70bb051aafeb5579f7e47cead99c2d985c2e8300f6142`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bd8c33d274f96ebb390618b02703a245dbec09e51cd487ec94b5f6c3dac042`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 930.8 KB (930822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8e1642af6d6db8e8ad3619ab4f5f428ef56619c0e876091ca0b4655a11965`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b57b9f16ec93912faeaec0afdcfc8b8cd1f798eda413061dd653df438b0d47`  
		Last Modified: Wed, 25 Nov 2020 23:24:05 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a598debd0e6f990ad14673192d3b379b053547d6568f44863e629abc8a39d2`  
		Last Modified: Wed, 25 Nov 2020 23:24:19 GMT  
		Size: 79.4 MB (79381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e237cd4e5fe3cb59ec0ce602c1ba748800154ce10cac5d679c9faa1611c07faa`  
		Last Modified: Wed, 25 Nov 2020 23:24:04 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282b9b89ce1ab00795ed0d76fff6c0ecbe3a6d37cfc7574d9076725862a6dc75`  
		Last Modified: Wed, 25 Nov 2020 23:24:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dc8f71c3eb6f5536186e4d147d3ad880a372299d309a7a953a0e2c8d77747465
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107605193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195be8b470b4c7f3a9241ca6ece8340384926572beeb6b9b32cd260b4e3a6a0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:32:47 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 04 Nov 2020 19:48:02 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 04 Nov 2020 19:48:04 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 04 Nov 2020 19:49:04 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 04 Nov 2020 19:49:07 GMT
VOLUME [/var/lib/mysql]
# Wed, 04 Nov 2020 19:49:07 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 04 Nov 2020 19:49:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 04 Nov 2020 19:49:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Nov 2020 19:49:11 GMT
EXPOSE 3306
# Wed, 04 Nov 2020 19:49:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40e91a70557f9b13296e1315d3e18476ae998791ab95cc0535611c31416de84`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c59b4cdb1026f1943894ced30677ef3d98d0b781dee583f614f7b3c606571`  
		Last Modified: Wed, 04 Nov 2020 19:52:06 GMT  
		Size: 77.3 MB (77289343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915478cebb19da9e0521a7a9ce22aeb0d26cd27b1dfd9b680c534783d6e0187f`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ddecdcf239cbe3b0ca269ba1c4e59731792aefb467ef4812fbd231dc66724c8`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9043d8ae5ba6b968c27fa68e64230bd65379b1367ec22c6f47af83f2f72c83a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120115469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a19a2236cd5768f94c87655b69ec5974b52bc279747abae0f2e70033588fd7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:30:16 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 04 Nov 2020 20:49:58 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 04 Nov 2020 20:50:11 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 04 Nov 2020 20:58:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 04 Nov 2020 20:58:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 04 Nov 2020 20:58:22 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 04 Nov 2020 20:58:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 04 Nov 2020 20:58:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Nov 2020 20:58:51 GMT
EXPOSE 3306
# Wed, 04 Nov 2020 20:58:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e6f1836379f3f02bfbdf5430817c013de79a3c7342ee5ba8a3d31f701fc3b`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffd392cd28ea555f1cfebde0c917e98752a880b3cf002a1597956a425263e7b`  
		Last Modified: Wed, 04 Nov 2020 21:02:52 GMT  
		Size: 81.9 MB (81885561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50f548b80e05319922ec0f03d07da193322a1cb4dc76edcceeda7d1a9b6ee66`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760e940662767a020cd4146178693567376905aed7ac153af59393d1b6b348e2`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48`

```console
$ docker pull mariadb@sha256:c1b13e294590066f390710d63f64324d5a42f5e0ba7680816f642e32727ee6f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48` - linux; amd64

```console
$ docker pull mariadb@sha256:aa5b677a55dae30f6c7694a63b92fb53988a8a241df09f7dc48bf8016c8f8388
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113172303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d374fe48b4e1d02456b69dfca8c49c4c6b70ef6565625813ba3ecae29c4ddc86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:20:10 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:20:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:20:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:20:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:20:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:21:26 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 25 Nov 2020 23:21:26 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 25 Nov 2020 23:21:27 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:22:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:22:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:22:02 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:22:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:22:04 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:22:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12260b0e97bc71b9bff6cd1af9e1c9c8bddccbc0e8c8198a4d49fc8bcec162e3`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a55695dfa04b41d261954f037febf6e4541519bd02fe4bdb1e48a0a7c4b31`  
		Last Modified: Wed, 25 Nov 2020 23:23:46 GMT  
		Size: 4.8 MB (4811249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b965e29cfef068223e351c81acb95c2305cf13e74ce8c12d82b7f4bfcc5042e`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 1.3 MB (1326975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013e2bd9bdd9019386d70bb051aafeb5579f7e47cead99c2d985c2e8300f6142`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bd8c33d274f96ebb390618b02703a245dbec09e51cd487ec94b5f6c3dac042`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 930.8 KB (930822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8e1642af6d6db8e8ad3619ab4f5f428ef56619c0e876091ca0b4655a11965`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b57b9f16ec93912faeaec0afdcfc8b8cd1f798eda413061dd653df438b0d47`  
		Last Modified: Wed, 25 Nov 2020 23:24:05 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a598debd0e6f990ad14673192d3b379b053547d6568f44863e629abc8a39d2`  
		Last Modified: Wed, 25 Nov 2020 23:24:19 GMT  
		Size: 79.4 MB (79381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e237cd4e5fe3cb59ec0ce602c1ba748800154ce10cac5d679c9faa1611c07faa`  
		Last Modified: Wed, 25 Nov 2020 23:24:04 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282b9b89ce1ab00795ed0d76fff6c0ecbe3a6d37cfc7574d9076725862a6dc75`  
		Last Modified: Wed, 25 Nov 2020 23:24:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dc8f71c3eb6f5536186e4d147d3ad880a372299d309a7a953a0e2c8d77747465
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107605193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195be8b470b4c7f3a9241ca6ece8340384926572beeb6b9b32cd260b4e3a6a0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:32:47 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 04 Nov 2020 19:48:02 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 04 Nov 2020 19:48:04 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 04 Nov 2020 19:49:04 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 04 Nov 2020 19:49:07 GMT
VOLUME [/var/lib/mysql]
# Wed, 04 Nov 2020 19:49:07 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 04 Nov 2020 19:49:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 04 Nov 2020 19:49:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Nov 2020 19:49:11 GMT
EXPOSE 3306
# Wed, 04 Nov 2020 19:49:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40e91a70557f9b13296e1315d3e18476ae998791ab95cc0535611c31416de84`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c59b4cdb1026f1943894ced30677ef3d98d0b781dee583f614f7b3c606571`  
		Last Modified: Wed, 04 Nov 2020 19:52:06 GMT  
		Size: 77.3 MB (77289343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915478cebb19da9e0521a7a9ce22aeb0d26cd27b1dfd9b680c534783d6e0187f`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ddecdcf239cbe3b0ca269ba1c4e59731792aefb467ef4812fbd231dc66724c8`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9043d8ae5ba6b968c27fa68e64230bd65379b1367ec22c6f47af83f2f72c83a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120115469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a19a2236cd5768f94c87655b69ec5974b52bc279747abae0f2e70033588fd7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:30:16 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 04 Nov 2020 20:49:58 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 04 Nov 2020 20:50:11 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 04 Nov 2020 20:58:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 04 Nov 2020 20:58:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 04 Nov 2020 20:58:22 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 04 Nov 2020 20:58:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 04 Nov 2020 20:58:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Nov 2020 20:58:51 GMT
EXPOSE 3306
# Wed, 04 Nov 2020 20:58:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e6f1836379f3f02bfbdf5430817c013de79a3c7342ee5ba8a3d31f701fc3b`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffd392cd28ea555f1cfebde0c917e98752a880b3cf002a1597956a425263e7b`  
		Last Modified: Wed, 04 Nov 2020 21:02:52 GMT  
		Size: 81.9 MB (81885561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50f548b80e05319922ec0f03d07da193322a1cb4dc76edcceeda7d1a9b6ee66`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760e940662767a020cd4146178693567376905aed7ac153af59393d1b6b348e2`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48-bionic`

```console
$ docker pull mariadb@sha256:c1b13e294590066f390710d63f64324d5a42f5e0ba7680816f642e32727ee6f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:aa5b677a55dae30f6c7694a63b92fb53988a8a241df09f7dc48bf8016c8f8388
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113172303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d374fe48b4e1d02456b69dfca8c49c4c6b70ef6565625813ba3ecae29c4ddc86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:20:10 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:20:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:20:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:20:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:20:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:21:26 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 25 Nov 2020 23:21:26 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 25 Nov 2020 23:21:27 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:22:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:22:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:22:02 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:22:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:22:04 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:22:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12260b0e97bc71b9bff6cd1af9e1c9c8bddccbc0e8c8198a4d49fc8bcec162e3`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a55695dfa04b41d261954f037febf6e4541519bd02fe4bdb1e48a0a7c4b31`  
		Last Modified: Wed, 25 Nov 2020 23:23:46 GMT  
		Size: 4.8 MB (4811249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b965e29cfef068223e351c81acb95c2305cf13e74ce8c12d82b7f4bfcc5042e`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 1.3 MB (1326975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013e2bd9bdd9019386d70bb051aafeb5579f7e47cead99c2d985c2e8300f6142`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bd8c33d274f96ebb390618b02703a245dbec09e51cd487ec94b5f6c3dac042`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 930.8 KB (930822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8e1642af6d6db8e8ad3619ab4f5f428ef56619c0e876091ca0b4655a11965`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b57b9f16ec93912faeaec0afdcfc8b8cd1f798eda413061dd653df438b0d47`  
		Last Modified: Wed, 25 Nov 2020 23:24:05 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a598debd0e6f990ad14673192d3b379b053547d6568f44863e629abc8a39d2`  
		Last Modified: Wed, 25 Nov 2020 23:24:19 GMT  
		Size: 79.4 MB (79381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e237cd4e5fe3cb59ec0ce602c1ba748800154ce10cac5d679c9faa1611c07faa`  
		Last Modified: Wed, 25 Nov 2020 23:24:04 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282b9b89ce1ab00795ed0d76fff6c0ecbe3a6d37cfc7574d9076725862a6dc75`  
		Last Modified: Wed, 25 Nov 2020 23:24:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dc8f71c3eb6f5536186e4d147d3ad880a372299d309a7a953a0e2c8d77747465
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107605193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195be8b470b4c7f3a9241ca6ece8340384926572beeb6b9b32cd260b4e3a6a0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:32:47 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 04 Nov 2020 19:48:02 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 04 Nov 2020 19:48:04 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 04 Nov 2020 19:49:04 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 04 Nov 2020 19:49:07 GMT
VOLUME [/var/lib/mysql]
# Wed, 04 Nov 2020 19:49:07 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 04 Nov 2020 19:49:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 04 Nov 2020 19:49:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Nov 2020 19:49:11 GMT
EXPOSE 3306
# Wed, 04 Nov 2020 19:49:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40e91a70557f9b13296e1315d3e18476ae998791ab95cc0535611c31416de84`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c59b4cdb1026f1943894ced30677ef3d98d0b781dee583f614f7b3c606571`  
		Last Modified: Wed, 04 Nov 2020 19:52:06 GMT  
		Size: 77.3 MB (77289343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915478cebb19da9e0521a7a9ce22aeb0d26cd27b1dfd9b680c534783d6e0187f`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ddecdcf239cbe3b0ca269ba1c4e59731792aefb467ef4812fbd231dc66724c8`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9043d8ae5ba6b968c27fa68e64230bd65379b1367ec22c6f47af83f2f72c83a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120115469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a19a2236cd5768f94c87655b69ec5974b52bc279747abae0f2e70033588fd7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:30:16 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 04 Nov 2020 20:49:58 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 04 Nov 2020 20:50:11 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 04 Nov 2020 20:58:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 04 Nov 2020 20:58:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 04 Nov 2020 20:58:22 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 04 Nov 2020 20:58:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 04 Nov 2020 20:58:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Nov 2020 20:58:51 GMT
EXPOSE 3306
# Wed, 04 Nov 2020 20:58:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e6f1836379f3f02bfbdf5430817c013de79a3c7342ee5ba8a3d31f701fc3b`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffd392cd28ea555f1cfebde0c917e98752a880b3cf002a1597956a425263e7b`  
		Last Modified: Wed, 04 Nov 2020 21:02:52 GMT  
		Size: 81.9 MB (81885561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50f548b80e05319922ec0f03d07da193322a1cb4dc76edcceeda7d1a9b6ee66`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760e940662767a020cd4146178693567376905aed7ac153af59393d1b6b348e2`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1-bionic`

```console
$ docker pull mariadb@sha256:c1b13e294590066f390710d63f64324d5a42f5e0ba7680816f642e32727ee6f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:aa5b677a55dae30f6c7694a63b92fb53988a8a241df09f7dc48bf8016c8f8388
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113172303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d374fe48b4e1d02456b69dfca8c49c4c6b70ef6565625813ba3ecae29c4ddc86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:20:10 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:20:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:20:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:20:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:20:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:21:26 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 25 Nov 2020 23:21:26 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 25 Nov 2020 23:21:27 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:22:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:22:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:22:02 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:22:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:22:04 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:22:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12260b0e97bc71b9bff6cd1af9e1c9c8bddccbc0e8c8198a4d49fc8bcec162e3`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a55695dfa04b41d261954f037febf6e4541519bd02fe4bdb1e48a0a7c4b31`  
		Last Modified: Wed, 25 Nov 2020 23:23:46 GMT  
		Size: 4.8 MB (4811249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b965e29cfef068223e351c81acb95c2305cf13e74ce8c12d82b7f4bfcc5042e`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 1.3 MB (1326975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013e2bd9bdd9019386d70bb051aafeb5579f7e47cead99c2d985c2e8300f6142`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bd8c33d274f96ebb390618b02703a245dbec09e51cd487ec94b5f6c3dac042`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 930.8 KB (930822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8e1642af6d6db8e8ad3619ab4f5f428ef56619c0e876091ca0b4655a11965`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b57b9f16ec93912faeaec0afdcfc8b8cd1f798eda413061dd653df438b0d47`  
		Last Modified: Wed, 25 Nov 2020 23:24:05 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a598debd0e6f990ad14673192d3b379b053547d6568f44863e629abc8a39d2`  
		Last Modified: Wed, 25 Nov 2020 23:24:19 GMT  
		Size: 79.4 MB (79381662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e237cd4e5fe3cb59ec0ce602c1ba748800154ce10cac5d679c9faa1611c07faa`  
		Last Modified: Wed, 25 Nov 2020 23:24:04 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282b9b89ce1ab00795ed0d76fff6c0ecbe3a6d37cfc7574d9076725862a6dc75`  
		Last Modified: Wed, 25 Nov 2020 23:24:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dc8f71c3eb6f5536186e4d147d3ad880a372299d309a7a953a0e2c8d77747465
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107605193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195be8b470b4c7f3a9241ca6ece8340384926572beeb6b9b32cd260b4e3a6a0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:32:47 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 04 Nov 2020 19:48:02 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 04 Nov 2020 19:48:04 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 04 Nov 2020 19:49:04 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 04 Nov 2020 19:49:07 GMT
VOLUME [/var/lib/mysql]
# Wed, 04 Nov 2020 19:49:07 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 04 Nov 2020 19:49:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 04 Nov 2020 19:49:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Nov 2020 19:49:11 GMT
EXPOSE 3306
# Wed, 04 Nov 2020 19:49:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40e91a70557f9b13296e1315d3e18476ae998791ab95cc0535611c31416de84`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c59b4cdb1026f1943894ced30677ef3d98d0b781dee583f614f7b3c606571`  
		Last Modified: Wed, 04 Nov 2020 19:52:06 GMT  
		Size: 77.3 MB (77289343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915478cebb19da9e0521a7a9ce22aeb0d26cd27b1dfd9b680c534783d6e0187f`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ddecdcf239cbe3b0ca269ba1c4e59731792aefb467ef4812fbd231dc66724c8`  
		Last Modified: Wed, 04 Nov 2020 19:51:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:9043d8ae5ba6b968c27fa68e64230bd65379b1367ec22c6f47af83f2f72c83a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120115469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a19a2236cd5768f94c87655b69ec5974b52bc279747abae0f2e70033588fd7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:30:16 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 04 Nov 2020 20:49:58 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Wed, 04 Nov 2020 20:50:11 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 04 Nov 2020 20:58:02 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 04 Nov 2020 20:58:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 04 Nov 2020 20:58:22 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 04 Nov 2020 20:58:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 04 Nov 2020 20:58:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 04 Nov 2020 20:58:51 GMT
EXPOSE 3306
# Wed, 04 Nov 2020 20:58:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005e6f1836379f3f02bfbdf5430817c013de79a3c7342ee5ba8a3d31f701fc3b`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffd392cd28ea555f1cfebde0c917e98752a880b3cf002a1597956a425263e7b`  
		Last Modified: Wed, 04 Nov 2020 21:02:52 GMT  
		Size: 81.9 MB (81885561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50f548b80e05319922ec0f03d07da193322a1cb4dc76edcceeda7d1a9b6ee66`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760e940662767a020cd4146178693567376905aed7ac153af59393d1b6b348e2`  
		Last Modified: Wed, 04 Nov 2020 21:02:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:1d504649f0895bc02ab7a62b046f2c45252e6d9bbca4bd967371efa24d1ea4e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:187b02ad495b0cc95662f3382bf8a811319b54d224bd12d24919988137de7cb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109013953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2cac908d8ed760a06c9b312aaac6d79cd27d73309f27b01290c57e207714832`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:20:10 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:20:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:20:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:20:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:20:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:20:42 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 25 Nov 2020 23:20:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 25 Nov 2020 23:20:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:21:19 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:21:19 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:21:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:21:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:21:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:21:21 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:21:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12260b0e97bc71b9bff6cd1af9e1c9c8bddccbc0e8c8198a4d49fc8bcec162e3`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a55695dfa04b41d261954f037febf6e4541519bd02fe4bdb1e48a0a7c4b31`  
		Last Modified: Wed, 25 Nov 2020 23:23:46 GMT  
		Size: 4.8 MB (4811249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b965e29cfef068223e351c81acb95c2305cf13e74ce8c12d82b7f4bfcc5042e`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 1.3 MB (1326975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013e2bd9bdd9019386d70bb051aafeb5579f7e47cead99c2d985c2e8300f6142`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bd8c33d274f96ebb390618b02703a245dbec09e51cd487ec94b5f6c3dac042`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 930.8 KB (930822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8e1642af6d6db8e8ad3619ab4f5f428ef56619c0e876091ca0b4655a11965`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0cf031acecbc156d9a7d3f42e4500a4332bcb752d2a7ee076fe975d6058b4b`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6de340383fe8cc5461cdba43a65d37d7bf488fbe55ee0d067b3b82de2486ab`  
		Last Modified: Wed, 25 Nov 2020 23:23:56 GMT  
		Size: 75.2 MB (75223313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a0c815551ab5c81673e3b60b0aa5075e92a8a442e75c75ab9dad3e0cdbf774`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa568cd01c082392d8fbe7bec079970ec6b0993d4a784575e9046e2946e46b82`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:129eba116f5cb2abe3d925e5e6d92dbb89911c6517236f2eca52f7a612d3f589
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105876251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3c548655367a5c7c696e540b002da804f2c355519364426fdfb6194e6c9fcfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:31:40 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 11 Nov 2020 21:44:10 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 11 Nov 2020 21:44:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:45:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:45:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:45:11 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:45:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:45:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:45:15 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:45:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb23248ab9fbf3672e5f0aa08b6456195ee261ec9fe104087256d60e735a302`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb18e506299f8bb91a49f00e3cab9cdf9e7b15d62ef2395d0e760d065fdad12`  
		Last Modified: Wed, 11 Nov 2020 21:48:11 GMT  
		Size: 75.6 MB (75560401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd8aeb10825d0a18755bbdfbfbb9658de1522b6bf511e0f5e9d6294b200ab94`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e464ca0920b63687cd9b50ea69648771704ff0b90425c40e4d417b758440826`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e829952dc845e4f8718e5cf368cadc68d2e468a5df61ccf10f16efec0cf3f4d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118163708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14da374cd8dbb396b6977c1f502d5df4e907ede1fc360b9971cd2d1bf801c412`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:27:33 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 11 Nov 2020 21:39:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 11 Nov 2020 21:40:03 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:47:05 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:47:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:47:24 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:47:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:47:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:48:06 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:48:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b155082608c3316667ec74f787abd888dd315d70a249827fe358d1e66d76ee8`  
		Last Modified: Wed, 11 Nov 2020 21:51:43 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d1e2b86c8fb862d18a86b6beda82deb4c4dce91daa888a0457785c51af78`  
		Last Modified: Wed, 11 Nov 2020 21:52:01 GMT  
		Size: 79.9 MB (79933798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e496e3179feef75d6a3435efb174197d23b766e0593736b4125d5e2ab37b6a1`  
		Last Modified: Wed, 11 Nov 2020 21:51:44 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00739d81c76ea99bfece98bfce71fb117be571c4480bc5e10c36f4fe2e87d35f`  
		Last Modified: Wed, 11 Nov 2020 21:51:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.36`

```console
$ docker pull mariadb@sha256:1d504649f0895bc02ab7a62b046f2c45252e6d9bbca4bd967371efa24d1ea4e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.36` - linux; amd64

```console
$ docker pull mariadb@sha256:187b02ad495b0cc95662f3382bf8a811319b54d224bd12d24919988137de7cb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109013953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2cac908d8ed760a06c9b312aaac6d79cd27d73309f27b01290c57e207714832`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:20:10 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:20:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:20:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:20:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:20:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:20:42 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 25 Nov 2020 23:20:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 25 Nov 2020 23:20:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:21:19 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:21:19 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:21:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:21:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:21:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:21:21 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:21:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12260b0e97bc71b9bff6cd1af9e1c9c8bddccbc0e8c8198a4d49fc8bcec162e3`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a55695dfa04b41d261954f037febf6e4541519bd02fe4bdb1e48a0a7c4b31`  
		Last Modified: Wed, 25 Nov 2020 23:23:46 GMT  
		Size: 4.8 MB (4811249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b965e29cfef068223e351c81acb95c2305cf13e74ce8c12d82b7f4bfcc5042e`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 1.3 MB (1326975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013e2bd9bdd9019386d70bb051aafeb5579f7e47cead99c2d985c2e8300f6142`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bd8c33d274f96ebb390618b02703a245dbec09e51cd487ec94b5f6c3dac042`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 930.8 KB (930822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8e1642af6d6db8e8ad3619ab4f5f428ef56619c0e876091ca0b4655a11965`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0cf031acecbc156d9a7d3f42e4500a4332bcb752d2a7ee076fe975d6058b4b`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6de340383fe8cc5461cdba43a65d37d7bf488fbe55ee0d067b3b82de2486ab`  
		Last Modified: Wed, 25 Nov 2020 23:23:56 GMT  
		Size: 75.2 MB (75223313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a0c815551ab5c81673e3b60b0aa5075e92a8a442e75c75ab9dad3e0cdbf774`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa568cd01c082392d8fbe7bec079970ec6b0993d4a784575e9046e2946e46b82`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.36` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:129eba116f5cb2abe3d925e5e6d92dbb89911c6517236f2eca52f7a612d3f589
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105876251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3c548655367a5c7c696e540b002da804f2c355519364426fdfb6194e6c9fcfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:31:40 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 11 Nov 2020 21:44:10 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 11 Nov 2020 21:44:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:45:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:45:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:45:11 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:45:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:45:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:45:15 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:45:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb23248ab9fbf3672e5f0aa08b6456195ee261ec9fe104087256d60e735a302`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb18e506299f8bb91a49f00e3cab9cdf9e7b15d62ef2395d0e760d065fdad12`  
		Last Modified: Wed, 11 Nov 2020 21:48:11 GMT  
		Size: 75.6 MB (75560401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd8aeb10825d0a18755bbdfbfbb9658de1522b6bf511e0f5e9d6294b200ab94`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e464ca0920b63687cd9b50ea69648771704ff0b90425c40e4d417b758440826`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.36` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e829952dc845e4f8718e5cf368cadc68d2e468a5df61ccf10f16efec0cf3f4d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118163708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14da374cd8dbb396b6977c1f502d5df4e907ede1fc360b9971cd2d1bf801c412`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:27:33 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 11 Nov 2020 21:39:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 11 Nov 2020 21:40:03 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:47:05 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:47:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:47:24 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:47:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:47:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:48:06 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:48:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b155082608c3316667ec74f787abd888dd315d70a249827fe358d1e66d76ee8`  
		Last Modified: Wed, 11 Nov 2020 21:51:43 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d1e2b86c8fb862d18a86b6beda82deb4c4dce91daa888a0457785c51af78`  
		Last Modified: Wed, 11 Nov 2020 21:52:01 GMT  
		Size: 79.9 MB (79933798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e496e3179feef75d6a3435efb174197d23b766e0593736b4125d5e2ab37b6a1`  
		Last Modified: Wed, 11 Nov 2020 21:51:44 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00739d81c76ea99bfece98bfce71fb117be571c4480bc5e10c36f4fe2e87d35f`  
		Last Modified: Wed, 11 Nov 2020 21:51:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.36-bionic`

```console
$ docker pull mariadb@sha256:1d504649f0895bc02ab7a62b046f2c45252e6d9bbca4bd967371efa24d1ea4e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.36-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:187b02ad495b0cc95662f3382bf8a811319b54d224bd12d24919988137de7cb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109013953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2cac908d8ed760a06c9b312aaac6d79cd27d73309f27b01290c57e207714832`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:20:10 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:20:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:20:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:20:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:20:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:20:42 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 25 Nov 2020 23:20:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 25 Nov 2020 23:20:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:21:19 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:21:19 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:21:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:21:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:21:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:21:21 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:21:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12260b0e97bc71b9bff6cd1af9e1c9c8bddccbc0e8c8198a4d49fc8bcec162e3`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a55695dfa04b41d261954f037febf6e4541519bd02fe4bdb1e48a0a7c4b31`  
		Last Modified: Wed, 25 Nov 2020 23:23:46 GMT  
		Size: 4.8 MB (4811249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b965e29cfef068223e351c81acb95c2305cf13e74ce8c12d82b7f4bfcc5042e`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 1.3 MB (1326975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013e2bd9bdd9019386d70bb051aafeb5579f7e47cead99c2d985c2e8300f6142`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bd8c33d274f96ebb390618b02703a245dbec09e51cd487ec94b5f6c3dac042`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 930.8 KB (930822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8e1642af6d6db8e8ad3619ab4f5f428ef56619c0e876091ca0b4655a11965`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0cf031acecbc156d9a7d3f42e4500a4332bcb752d2a7ee076fe975d6058b4b`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6de340383fe8cc5461cdba43a65d37d7bf488fbe55ee0d067b3b82de2486ab`  
		Last Modified: Wed, 25 Nov 2020 23:23:56 GMT  
		Size: 75.2 MB (75223313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a0c815551ab5c81673e3b60b0aa5075e92a8a442e75c75ab9dad3e0cdbf774`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa568cd01c082392d8fbe7bec079970ec6b0993d4a784575e9046e2946e46b82`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.36-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:129eba116f5cb2abe3d925e5e6d92dbb89911c6517236f2eca52f7a612d3f589
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105876251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3c548655367a5c7c696e540b002da804f2c355519364426fdfb6194e6c9fcfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:31:40 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 11 Nov 2020 21:44:10 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 11 Nov 2020 21:44:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:45:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:45:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:45:11 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:45:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:45:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:45:15 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:45:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb23248ab9fbf3672e5f0aa08b6456195ee261ec9fe104087256d60e735a302`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb18e506299f8bb91a49f00e3cab9cdf9e7b15d62ef2395d0e760d065fdad12`  
		Last Modified: Wed, 11 Nov 2020 21:48:11 GMT  
		Size: 75.6 MB (75560401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd8aeb10825d0a18755bbdfbfbb9658de1522b6bf511e0f5e9d6294b200ab94`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e464ca0920b63687cd9b50ea69648771704ff0b90425c40e4d417b758440826`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.36-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e829952dc845e4f8718e5cf368cadc68d2e468a5df61ccf10f16efec0cf3f4d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118163708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14da374cd8dbb396b6977c1f502d5df4e907ede1fc360b9971cd2d1bf801c412`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:27:33 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 11 Nov 2020 21:39:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 11 Nov 2020 21:40:03 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:47:05 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:47:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:47:24 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:47:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:47:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:48:06 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:48:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b155082608c3316667ec74f787abd888dd315d70a249827fe358d1e66d76ee8`  
		Last Modified: Wed, 11 Nov 2020 21:51:43 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d1e2b86c8fb862d18a86b6beda82deb4c4dce91daa888a0457785c51af78`  
		Last Modified: Wed, 11 Nov 2020 21:52:01 GMT  
		Size: 79.9 MB (79933798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e496e3179feef75d6a3435efb174197d23b766e0593736b4125d5e2ab37b6a1`  
		Last Modified: Wed, 11 Nov 2020 21:51:44 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00739d81c76ea99bfece98bfce71fb117be571c4480bc5e10c36f4fe2e87d35f`  
		Last Modified: Wed, 11 Nov 2020 21:51:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:1d504649f0895bc02ab7a62b046f2c45252e6d9bbca4bd967371efa24d1ea4e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:187b02ad495b0cc95662f3382bf8a811319b54d224bd12d24919988137de7cb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109013953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2cac908d8ed760a06c9b312aaac6d79cd27d73309f27b01290c57e207714832`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:20:10 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:20:20 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:20:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:20:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:20:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:20:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:20:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:20:42 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 25 Nov 2020 23:20:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 25 Nov 2020 23:20:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:21:19 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:21:19 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:21:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:21:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:21:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:21:21 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:21:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12260b0e97bc71b9bff6cd1af9e1c9c8bddccbc0e8c8198a4d49fc8bcec162e3`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a55695dfa04b41d261954f037febf6e4541519bd02fe4bdb1e48a0a7c4b31`  
		Last Modified: Wed, 25 Nov 2020 23:23:46 GMT  
		Size: 4.8 MB (4811249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b965e29cfef068223e351c81acb95c2305cf13e74ce8c12d82b7f4bfcc5042e`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 1.3 MB (1326975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013e2bd9bdd9019386d70bb051aafeb5579f7e47cead99c2d985c2e8300f6142`  
		Last Modified: Wed, 25 Nov 2020 23:23:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bd8c33d274f96ebb390618b02703a245dbec09e51cd487ec94b5f6c3dac042`  
		Last Modified: Wed, 25 Nov 2020 23:23:43 GMT  
		Size: 930.8 KB (930822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc8e1642af6d6db8e8ad3619ab4f5f428ef56619c0e876091ca0b4655a11965`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0cf031acecbc156d9a7d3f42e4500a4332bcb752d2a7ee076fe975d6058b4b`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6de340383fe8cc5461cdba43a65d37d7bf488fbe55ee0d067b3b82de2486ab`  
		Last Modified: Wed, 25 Nov 2020 23:23:56 GMT  
		Size: 75.2 MB (75223313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a0c815551ab5c81673e3b60b0aa5075e92a8a442e75c75ab9dad3e0cdbf774`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa568cd01c082392d8fbe7bec079970ec6b0993d4a784575e9046e2946e46b82`  
		Last Modified: Wed, 25 Nov 2020 23:23:41 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:129eba116f5cb2abe3d925e5e6d92dbb89911c6517236f2eca52f7a612d3f589
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105876251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3c548655367a5c7c696e540b002da804f2c355519364426fdfb6194e6c9fcfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 22:47:32 GMT
ADD file:d2c57bfbb29f6de3b29050a2c50c3806e0c8caa26f6d8dea47f479c923d72e3e in / 
# Fri, 25 Sep 2020 22:47:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:47:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:47:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:47:39 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:30:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 25 Sep 2020 23:31:03 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:04 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Sep 2020 23:31:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Sep 2020 23:31:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Sep 2020 23:31:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 23:31:37 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 25 Sep 2020 23:31:40 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 25 Sep 2020 23:31:40 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 11 Nov 2020 21:44:10 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 11 Nov 2020 21:44:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:45:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:45:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:45:11 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:45:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:45:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:45:15 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:45:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:296c9ad75beec603486f1373addae8e2c509e94c4adda44c1289792c91624acc`  
		Last Modified: Tue, 22 Sep 2020 00:25:11 GMT  
		Size: 23.7 MB (23722853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0533d1393025aa8c38e0823a6546a0d4e5dec6b8b670758c25494c35783668d`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c11bb34abc87247c6a70c928b7a5ef4cd48093642eb0c4b8121a674d3e278c6`  
		Last Modified: Fri, 25 Sep 2020 22:49:19 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870b948e33cebad9af1f4cc77312dcfad86464dd571ed4ecb6e3880b64abd285`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d78577b121ac4f4d8a9a8fecaf3c849e9aa15ee980318138e60672a5dd85de`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 4.4 MB (4394361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fe0c4c88086ceb1b4f120de94964bd6050d51ab27eb80b76f6e71e9eb6fb2`  
		Last Modified: Fri, 25 Sep 2020 23:36:25 GMT  
		Size: 1.3 MB (1263464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456657275618d9347e2c3164308bfd0c90e1995e858896621d3b64c520aac55e`  
		Last Modified: Fri, 25 Sep 2020 23:36:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297f39adae4458e94ebfe715a0dd77d750580f8c6fd7961365c46778f415776c`  
		Last Modified: Fri, 25 Sep 2020 23:36:24 GMT  
		Size: 921.6 KB (921557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381305efa4d2f972fc7b3f6d8da8d7285f7aee1a3f4d6db3cf59e1695dabbc79`  
		Last Modified: Fri, 25 Sep 2020 23:36:21 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb23248ab9fbf3672e5f0aa08b6456195ee261ec9fe104087256d60e735a302`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb18e506299f8bb91a49f00e3cab9cdf9e7b15d62ef2395d0e760d065fdad12`  
		Last Modified: Wed, 11 Nov 2020 21:48:11 GMT  
		Size: 75.6 MB (75560401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd8aeb10825d0a18755bbdfbfbb9658de1522b6bf511e0f5e9d6294b200ab94`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e464ca0920b63687cd9b50ea69648771704ff0b90425c40e4d417b758440826`  
		Last Modified: Wed, 11 Nov 2020 21:47:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:e829952dc845e4f8718e5cf368cadc68d2e468a5df61ccf10f16efec0cf3f4d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118163708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14da374cd8dbb396b6977c1f502d5df4e907ede1fc360b9971cd2d1bf801c412`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:24:42 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 26 Sep 2020 04:26:12 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:26:16 GMT
ENV GOSU_VERSION=1.12
# Sat, 26 Sep 2020 04:26:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 26 Sep 2020 04:27:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 26 Sep 2020 04:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Sep 2020 04:27:25 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Sat, 26 Sep 2020 04:27:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Sat, 26 Sep 2020 04:27:33 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 11 Nov 2020 21:39:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Wed, 11 Nov 2020 21:40:03 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:47:05 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:47:20 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:47:24 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:47:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:47:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:48:06 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:48:15 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bce23f21744d3f5a1047249d677d9394faaf1f984f7ec4a9c1198277e1f3d18`  
		Last Modified: Sat, 26 Sep 2020 04:36:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d8cd57b26b1e7a1dd53588ecbabb82238fd04c435cabb3aeabc11d7aac7de1`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 5.6 MB (5629583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf63ae75dfbc766239bf488cddba751e125654cb6547cae7ba1227b0036e41`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 1.2 MB (1246387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe7724a4befdb4e6fb4a984e5531a59f4e2f18bca9eb68c1540e5c553d1cbe`  
		Last Modified: Sat, 26 Sep 2020 04:36:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110b905a4cfb8b9a52b8a48813cefc23379dca2ac8f646406490c42fcf4439d`  
		Last Modified: Sat, 26 Sep 2020 04:36:42 GMT  
		Size: 931.8 KB (931831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87b865ce6681ed862606042058bc38215b7d355bd89a5c0f648672f0f23259`  
		Last Modified: Sat, 26 Sep 2020 04:36:37 GMT  
		Size: 5.2 KB (5176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b155082608c3316667ec74f787abd888dd315d70a249827fe358d1e66d76ee8`  
		Last Modified: Wed, 11 Nov 2020 21:51:43 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5827d1e2b86c8fb862d18a86b6beda82deb4c4dce91daa888a0457785c51af78`  
		Last Modified: Wed, 11 Nov 2020 21:52:01 GMT  
		Size: 79.9 MB (79933798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e496e3179feef75d6a3435efb174197d23b766e0593736b4125d5e2ab37b6a1`  
		Last Modified: Wed, 11 Nov 2020 21:51:44 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00739d81c76ea99bfece98bfce71fb117be571c4480bc5e10c36f4fe2e87d35f`  
		Last Modified: Wed, 11 Nov 2020 21:51:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:379d3c3f3535de2cb183cedf74e3a2624d72a2bceb3decbd262b04db94b80ccc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:c6b30d896f477a6aaf63d7cafcb61fc9abe25a53ebed4ecc11f599a614b211c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119240111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e026e56f5f5543984af4fe5645753cd0218796a3d5c099e200c411ae2af8744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:19:29 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 25 Nov 2020 23:19:29 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 25 Nov 2020 23:19:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:19:58 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:19:59 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:19:59 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:20:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:20:00 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:20:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739c71d82551fa6496c93332a6cec5452acf3585131eaa3088c2e7d5e39266cf`  
		Last Modified: Wed, 25 Nov 2020 23:23:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65465f3a9066efc264c354405b6699d8c65da8bc703262377bfdcf99e860d004`  
		Last Modified: Wed, 25 Nov 2020 23:23:34 GMT  
		Size: 82.6 MB (82585390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d96eca58ffee80d5bd2cd68c4b19c2adc6f05ad56548433dce93d567c543974`  
		Last Modified: Wed, 25 Nov 2020 23:23:19 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ddb412bd222450b76a6571a8d775a29d2a703c4b2e72e4ee72278b6fc84437`  
		Last Modified: Wed, 25 Nov 2020 23:23:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:059ff07572870fc904fc333a216114a60d253551736a5ec11aad719bed77037a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (119005631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f82bb012b1c91e966f1c39f4e17d4312162c9b44433a53ab55909878e93294e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:37:03 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 11 Nov 2020 21:42:51 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 11 Nov 2020 21:42:52 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:43:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:43:49 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:43:49 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:43:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:43:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:43:53 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:43:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736acd09379c3b3a313254eb6b4aec878187a64c799e33b1fa6a13485a34dd3`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3730dd3dc1d9e42d6ee307aea1e0604a62635d54067b223b8b46a6e211af77`  
		Last Modified: Wed, 11 Nov 2020 21:47:39 GMT  
		Size: 83.8 MB (83847535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95adfcf57cc3dc78f114784c517f713d3be7e16242bd6524913938f973f302c1`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3046df25cd4713264a8c0e48c08e83ea58aabc180cc63f16e6c88454e982cbd8`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:092a477468febaba7104511f7225ae189453af89630760570794dd55bcb3bf7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131362825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9a64515d87311777ce4b1152b374a4bfad9a28099b9828e83aaa7849b9fbcc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:17:20 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 11 Nov 2020 21:32:42 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 11 Nov 2020 21:33:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:38:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:38:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:38:43 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:38:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:39:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:39:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3128572953ba5e77e473082ca349a5fa708ac41f8d51cad66d295eef1755d61`  
		Last Modified: Wed, 11 Nov 2020 21:51:01 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39313a0a34e6e154c580325d8b92a9a4e08ee4f0a693fa2a58db26d5963b1a58`  
		Last Modified: Wed, 11 Nov 2020 21:51:23 GMT  
		Size: 88.9 MB (88889687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec065186bff1f103cba26d17651b614742cefcf23af8b9d9b0ace27a911cc332`  
		Last Modified: Wed, 11 Nov 2020 21:51:02 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7f62b2bc83f1cf254231ae7a00b347e55231bd2bb4df109df7c82cf13cd68b`  
		Last Modified: Wed, 11 Nov 2020 21:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.27`

```console
$ docker pull mariadb@sha256:379d3c3f3535de2cb183cedf74e3a2624d72a2bceb3decbd262b04db94b80ccc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.27` - linux; amd64

```console
$ docker pull mariadb@sha256:c6b30d896f477a6aaf63d7cafcb61fc9abe25a53ebed4ecc11f599a614b211c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119240111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e026e56f5f5543984af4fe5645753cd0218796a3d5c099e200c411ae2af8744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:19:29 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 25 Nov 2020 23:19:29 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 25 Nov 2020 23:19:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:19:58 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:19:59 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:19:59 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:20:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:20:00 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:20:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739c71d82551fa6496c93332a6cec5452acf3585131eaa3088c2e7d5e39266cf`  
		Last Modified: Wed, 25 Nov 2020 23:23:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65465f3a9066efc264c354405b6699d8c65da8bc703262377bfdcf99e860d004`  
		Last Modified: Wed, 25 Nov 2020 23:23:34 GMT  
		Size: 82.6 MB (82585390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d96eca58ffee80d5bd2cd68c4b19c2adc6f05ad56548433dce93d567c543974`  
		Last Modified: Wed, 25 Nov 2020 23:23:19 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ddb412bd222450b76a6571a8d775a29d2a703c4b2e72e4ee72278b6fc84437`  
		Last Modified: Wed, 25 Nov 2020 23:23:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.27` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:059ff07572870fc904fc333a216114a60d253551736a5ec11aad719bed77037a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (119005631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f82bb012b1c91e966f1c39f4e17d4312162c9b44433a53ab55909878e93294e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:37:03 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 11 Nov 2020 21:42:51 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 11 Nov 2020 21:42:52 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:43:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:43:49 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:43:49 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:43:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:43:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:43:53 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:43:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736acd09379c3b3a313254eb6b4aec878187a64c799e33b1fa6a13485a34dd3`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3730dd3dc1d9e42d6ee307aea1e0604a62635d54067b223b8b46a6e211af77`  
		Last Modified: Wed, 11 Nov 2020 21:47:39 GMT  
		Size: 83.8 MB (83847535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95adfcf57cc3dc78f114784c517f713d3be7e16242bd6524913938f973f302c1`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3046df25cd4713264a8c0e48c08e83ea58aabc180cc63f16e6c88454e982cbd8`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.27` - linux; ppc64le

```console
$ docker pull mariadb@sha256:092a477468febaba7104511f7225ae189453af89630760570794dd55bcb3bf7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131362825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9a64515d87311777ce4b1152b374a4bfad9a28099b9828e83aaa7849b9fbcc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:17:20 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 11 Nov 2020 21:32:42 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 11 Nov 2020 21:33:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:38:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:38:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:38:43 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:38:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:39:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:39:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3128572953ba5e77e473082ca349a5fa708ac41f8d51cad66d295eef1755d61`  
		Last Modified: Wed, 11 Nov 2020 21:51:01 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39313a0a34e6e154c580325d8b92a9a4e08ee4f0a693fa2a58db26d5963b1a58`  
		Last Modified: Wed, 11 Nov 2020 21:51:23 GMT  
		Size: 88.9 MB (88889687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec065186bff1f103cba26d17651b614742cefcf23af8b9d9b0ace27a911cc332`  
		Last Modified: Wed, 11 Nov 2020 21:51:02 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7f62b2bc83f1cf254231ae7a00b347e55231bd2bb4df109df7c82cf13cd68b`  
		Last Modified: Wed, 11 Nov 2020 21:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.27-focal`

```console
$ docker pull mariadb@sha256:379d3c3f3535de2cb183cedf74e3a2624d72a2bceb3decbd262b04db94b80ccc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.27-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c6b30d896f477a6aaf63d7cafcb61fc9abe25a53ebed4ecc11f599a614b211c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119240111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e026e56f5f5543984af4fe5645753cd0218796a3d5c099e200c411ae2af8744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:19:29 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 25 Nov 2020 23:19:29 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 25 Nov 2020 23:19:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:19:58 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:19:59 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:19:59 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:20:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:20:00 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:20:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739c71d82551fa6496c93332a6cec5452acf3585131eaa3088c2e7d5e39266cf`  
		Last Modified: Wed, 25 Nov 2020 23:23:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65465f3a9066efc264c354405b6699d8c65da8bc703262377bfdcf99e860d004`  
		Last Modified: Wed, 25 Nov 2020 23:23:34 GMT  
		Size: 82.6 MB (82585390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d96eca58ffee80d5bd2cd68c4b19c2adc6f05ad56548433dce93d567c543974`  
		Last Modified: Wed, 25 Nov 2020 23:23:19 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ddb412bd222450b76a6571a8d775a29d2a703c4b2e72e4ee72278b6fc84437`  
		Last Modified: Wed, 25 Nov 2020 23:23:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.27-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:059ff07572870fc904fc333a216114a60d253551736a5ec11aad719bed77037a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (119005631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f82bb012b1c91e966f1c39f4e17d4312162c9b44433a53ab55909878e93294e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:37:03 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 11 Nov 2020 21:42:51 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 11 Nov 2020 21:42:52 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:43:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:43:49 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:43:49 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:43:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:43:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:43:53 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:43:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736acd09379c3b3a313254eb6b4aec878187a64c799e33b1fa6a13485a34dd3`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3730dd3dc1d9e42d6ee307aea1e0604a62635d54067b223b8b46a6e211af77`  
		Last Modified: Wed, 11 Nov 2020 21:47:39 GMT  
		Size: 83.8 MB (83847535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95adfcf57cc3dc78f114784c517f713d3be7e16242bd6524913938f973f302c1`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3046df25cd4713264a8c0e48c08e83ea58aabc180cc63f16e6c88454e982cbd8`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.27-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:092a477468febaba7104511f7225ae189453af89630760570794dd55bcb3bf7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131362825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9a64515d87311777ce4b1152b374a4bfad9a28099b9828e83aaa7849b9fbcc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:17:20 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 11 Nov 2020 21:32:42 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 11 Nov 2020 21:33:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:38:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:38:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:38:43 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:38:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:39:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:39:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3128572953ba5e77e473082ca349a5fa708ac41f8d51cad66d295eef1755d61`  
		Last Modified: Wed, 11 Nov 2020 21:51:01 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39313a0a34e6e154c580325d8b92a9a4e08ee4f0a693fa2a58db26d5963b1a58`  
		Last Modified: Wed, 11 Nov 2020 21:51:23 GMT  
		Size: 88.9 MB (88889687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec065186bff1f103cba26d17651b614742cefcf23af8b9d9b0ace27a911cc332`  
		Last Modified: Wed, 11 Nov 2020 21:51:02 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7f62b2bc83f1cf254231ae7a00b347e55231bd2bb4df109df7c82cf13cd68b`  
		Last Modified: Wed, 11 Nov 2020 21:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:379d3c3f3535de2cb183cedf74e3a2624d72a2bceb3decbd262b04db94b80ccc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:c6b30d896f477a6aaf63d7cafcb61fc9abe25a53ebed4ecc11f599a614b211c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119240111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e026e56f5f5543984af4fe5645753cd0218796a3d5c099e200c411ae2af8744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:19:29 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 25 Nov 2020 23:19:29 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 25 Nov 2020 23:19:31 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:19:58 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:19:59 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:19:59 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:20:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:20:00 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:20:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739c71d82551fa6496c93332a6cec5452acf3585131eaa3088c2e7d5e39266cf`  
		Last Modified: Wed, 25 Nov 2020 23:23:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65465f3a9066efc264c354405b6699d8c65da8bc703262377bfdcf99e860d004`  
		Last Modified: Wed, 25 Nov 2020 23:23:34 GMT  
		Size: 82.6 MB (82585390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d96eca58ffee80d5bd2cd68c4b19c2adc6f05ad56548433dce93d567c543974`  
		Last Modified: Wed, 25 Nov 2020 23:23:19 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ddb412bd222450b76a6571a8d775a29d2a703c4b2e72e4ee72278b6fc84437`  
		Last Modified: Wed, 25 Nov 2020 23:23:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:059ff07572870fc904fc333a216114a60d253551736a5ec11aad719bed77037a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (119005631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f82bb012b1c91e966f1c39f4e17d4312162c9b44433a53ab55909878e93294e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:37:03 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 11 Nov 2020 21:42:51 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 11 Nov 2020 21:42:52 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:43:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:43:49 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:43:49 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:43:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:43:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:43:53 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:43:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a736acd09379c3b3a313254eb6b4aec878187a64c799e33b1fa6a13485a34dd3`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3730dd3dc1d9e42d6ee307aea1e0604a62635d54067b223b8b46a6e211af77`  
		Last Modified: Wed, 11 Nov 2020 21:47:39 GMT  
		Size: 83.8 MB (83847535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95adfcf57cc3dc78f114784c517f713d3be7e16242bd6524913938f973f302c1`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3046df25cd4713264a8c0e48c08e83ea58aabc180cc63f16e6c88454e982cbd8`  
		Last Modified: Wed, 11 Nov 2020 21:47:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:092a477468febaba7104511f7225ae189453af89630760570794dd55bcb3bf7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131362825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b9a64515d87311777ce4b1152b374a4bfad9a28099b9828e83aaa7849b9fbcc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:17:20 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 11 Nov 2020 21:32:42 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Wed, 11 Nov 2020 21:33:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:38:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:38:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:38:43 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:38:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:39:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:39:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3128572953ba5e77e473082ca349a5fa708ac41f8d51cad66d295eef1755d61`  
		Last Modified: Wed, 11 Nov 2020 21:51:01 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39313a0a34e6e154c580325d8b92a9a4e08ee4f0a693fa2a58db26d5963b1a58`  
		Last Modified: Wed, 11 Nov 2020 21:51:23 GMT  
		Size: 88.9 MB (88889687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec065186bff1f103cba26d17651b614742cefcf23af8b9d9b0ace27a911cc332`  
		Last Modified: Wed, 11 Nov 2020 21:51:02 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7f62b2bc83f1cf254231ae7a00b347e55231bd2bb4df109df7c82cf13cd68b`  
		Last Modified: Wed, 11 Nov 2020 21:51:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:c0d2012709484678c0d1aa5ac0e0e46debe0591ddd0a4dedcbb85066702db649
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:8ba28db6cdc5f87b59e4be6c5724d26a11af70b62134f7142b4ef9fd382ef946
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123571140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b89851205aa235471ff68c8daf0701fae60ecb17c385246699e51f5c0eed3ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:18:48 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 25 Nov 2020 23:18:49 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 25 Nov 2020 23:18:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:19:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:19:21 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:19:21 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:19:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:19:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:19:23 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:19:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd7f0f336d95becc54d7a8b9f7228d46f8dece45218d848109e53c68ea5c8d2`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d455564f5ab63825e4ba7bbe83d44d1f6df04ad7ad11685744303f4e2b8a6d1`  
		Last Modified: Wed, 25 Nov 2020 23:23:11 GMT  
		Size: 86.9 MB (86916418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d384b4810a94b2a0ba6992a4c224f8c5840f6228feda6d71d13b636ebfc20f4`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2e7c2c7df1c88aa47353e1f5bbc1ffe7b2464e1df78143f2638a9e3b61a1dd`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c28cf25f78c7bbfa24896ba86309b733e6cfe7bc74da2ea3f2bcce0f82d2dca8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123322814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1338e0ee6f662e7c6c28a442838755c18e112268d2edd888b63c5f5cc8c3d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:35:44 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 11 Nov 2020 21:41:32 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 11 Nov 2020 21:41:34 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:42:29 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:42:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:42:32 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:42:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:42:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:42:36 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:42:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a8421f1a1c760507f6e74ce9090cf4fc5f02231f8c1e2634466fef53dd87d`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbacf27f433c06bdfc4a670d9dce4f2a90423b22743b0bfc82a4e7c8a1df4755`  
		Last Modified: Wed, 11 Nov 2020 21:46:56 GMT  
		Size: 88.2 MB (88164721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfeb4eae3c084535b956fff6deed5f955143be859f2e0cde0f60fdc995bf21a`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62fa358c0199b25937629991bf28a1bc6136e9f3cdd83ae5ce9845a73a7e6c`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f566897a5981e4fac1713f7aeb8c8aeac8cdced021ef4b0bc07988fca2df5e94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135815909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4698c4cc945a17ebad437bccc342fd4d66f31611b2e65be306d4f4beb1c5f3fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:09:21 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 11 Nov 2020 21:24:57 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 11 Nov 2020 21:25:08 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:31:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:31:41 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:31:47 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:31:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:32:11 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:32:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b315cab93312c5208f46751dc1a4a4e8a98a975507780b22f6d62a581ab6c10`  
		Last Modified: Wed, 11 Nov 2020 21:50:18 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7474eb0da552af0997e1190c05abe7cd5e25450835827dc05a9a67e4723a0e`  
		Last Modified: Wed, 11 Nov 2020 21:50:38 GMT  
		Size: 93.3 MB (93342769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732377b864d33f75b094fe90eac7cf17807e1ffe2709b5929237d32e24c2351`  
		Last Modified: Wed, 11 Nov 2020 21:50:18 GMT  
		Size: 4.9 KB (4920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d226da7be978e457796e2e372bc77f0e9a44ccb95bbaba2c0bf7c610d845d349`  
		Last Modified: Wed, 11 Nov 2020 21:50:17 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.17`

```console
$ docker pull mariadb@sha256:c0d2012709484678c0d1aa5ac0e0e46debe0591ddd0a4dedcbb85066702db649
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.17` - linux; amd64

```console
$ docker pull mariadb@sha256:8ba28db6cdc5f87b59e4be6c5724d26a11af70b62134f7142b4ef9fd382ef946
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123571140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b89851205aa235471ff68c8daf0701fae60ecb17c385246699e51f5c0eed3ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:18:48 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 25 Nov 2020 23:18:49 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 25 Nov 2020 23:18:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:19:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:19:21 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:19:21 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:19:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:19:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:19:23 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:19:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd7f0f336d95becc54d7a8b9f7228d46f8dece45218d848109e53c68ea5c8d2`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d455564f5ab63825e4ba7bbe83d44d1f6df04ad7ad11685744303f4e2b8a6d1`  
		Last Modified: Wed, 25 Nov 2020 23:23:11 GMT  
		Size: 86.9 MB (86916418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d384b4810a94b2a0ba6992a4c224f8c5840f6228feda6d71d13b636ebfc20f4`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2e7c2c7df1c88aa47353e1f5bbc1ffe7b2464e1df78143f2638a9e3b61a1dd`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.17` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c28cf25f78c7bbfa24896ba86309b733e6cfe7bc74da2ea3f2bcce0f82d2dca8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123322814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1338e0ee6f662e7c6c28a442838755c18e112268d2edd888b63c5f5cc8c3d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:35:44 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 11 Nov 2020 21:41:32 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 11 Nov 2020 21:41:34 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:42:29 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:42:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:42:32 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:42:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:42:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:42:36 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:42:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a8421f1a1c760507f6e74ce9090cf4fc5f02231f8c1e2634466fef53dd87d`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbacf27f433c06bdfc4a670d9dce4f2a90423b22743b0bfc82a4e7c8a1df4755`  
		Last Modified: Wed, 11 Nov 2020 21:46:56 GMT  
		Size: 88.2 MB (88164721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfeb4eae3c084535b956fff6deed5f955143be859f2e0cde0f60fdc995bf21a`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62fa358c0199b25937629991bf28a1bc6136e9f3cdd83ae5ce9845a73a7e6c`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.17` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f566897a5981e4fac1713f7aeb8c8aeac8cdced021ef4b0bc07988fca2df5e94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135815909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4698c4cc945a17ebad437bccc342fd4d66f31611b2e65be306d4f4beb1c5f3fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:09:21 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 11 Nov 2020 21:24:57 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 11 Nov 2020 21:25:08 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:31:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:31:41 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:31:47 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:31:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:32:11 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:32:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b315cab93312c5208f46751dc1a4a4e8a98a975507780b22f6d62a581ab6c10`  
		Last Modified: Wed, 11 Nov 2020 21:50:18 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7474eb0da552af0997e1190c05abe7cd5e25450835827dc05a9a67e4723a0e`  
		Last Modified: Wed, 11 Nov 2020 21:50:38 GMT  
		Size: 93.3 MB (93342769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732377b864d33f75b094fe90eac7cf17807e1ffe2709b5929237d32e24c2351`  
		Last Modified: Wed, 11 Nov 2020 21:50:18 GMT  
		Size: 4.9 KB (4920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d226da7be978e457796e2e372bc77f0e9a44ccb95bbaba2c0bf7c610d845d349`  
		Last Modified: Wed, 11 Nov 2020 21:50:17 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.17-focal`

```console
$ docker pull mariadb@sha256:c0d2012709484678c0d1aa5ac0e0e46debe0591ddd0a4dedcbb85066702db649
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.17-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:8ba28db6cdc5f87b59e4be6c5724d26a11af70b62134f7142b4ef9fd382ef946
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123571140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b89851205aa235471ff68c8daf0701fae60ecb17c385246699e51f5c0eed3ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:18:48 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 25 Nov 2020 23:18:49 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 25 Nov 2020 23:18:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:19:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:19:21 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:19:21 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:19:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:19:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:19:23 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:19:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd7f0f336d95becc54d7a8b9f7228d46f8dece45218d848109e53c68ea5c8d2`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d455564f5ab63825e4ba7bbe83d44d1f6df04ad7ad11685744303f4e2b8a6d1`  
		Last Modified: Wed, 25 Nov 2020 23:23:11 GMT  
		Size: 86.9 MB (86916418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d384b4810a94b2a0ba6992a4c224f8c5840f6228feda6d71d13b636ebfc20f4`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2e7c2c7df1c88aa47353e1f5bbc1ffe7b2464e1df78143f2638a9e3b61a1dd`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.17-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c28cf25f78c7bbfa24896ba86309b733e6cfe7bc74da2ea3f2bcce0f82d2dca8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123322814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1338e0ee6f662e7c6c28a442838755c18e112268d2edd888b63c5f5cc8c3d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:35:44 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 11 Nov 2020 21:41:32 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 11 Nov 2020 21:41:34 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:42:29 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:42:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:42:32 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:42:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:42:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:42:36 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:42:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a8421f1a1c760507f6e74ce9090cf4fc5f02231f8c1e2634466fef53dd87d`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbacf27f433c06bdfc4a670d9dce4f2a90423b22743b0bfc82a4e7c8a1df4755`  
		Last Modified: Wed, 11 Nov 2020 21:46:56 GMT  
		Size: 88.2 MB (88164721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfeb4eae3c084535b956fff6deed5f955143be859f2e0cde0f60fdc995bf21a`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62fa358c0199b25937629991bf28a1bc6136e9f3cdd83ae5ce9845a73a7e6c`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.17-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f566897a5981e4fac1713f7aeb8c8aeac8cdced021ef4b0bc07988fca2df5e94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135815909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4698c4cc945a17ebad437bccc342fd4d66f31611b2e65be306d4f4beb1c5f3fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:09:21 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 11 Nov 2020 21:24:57 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 11 Nov 2020 21:25:08 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:31:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:31:41 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:31:47 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:31:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:32:11 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:32:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b315cab93312c5208f46751dc1a4a4e8a98a975507780b22f6d62a581ab6c10`  
		Last Modified: Wed, 11 Nov 2020 21:50:18 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7474eb0da552af0997e1190c05abe7cd5e25450835827dc05a9a67e4723a0e`  
		Last Modified: Wed, 11 Nov 2020 21:50:38 GMT  
		Size: 93.3 MB (93342769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732377b864d33f75b094fe90eac7cf17807e1ffe2709b5929237d32e24c2351`  
		Last Modified: Wed, 11 Nov 2020 21:50:18 GMT  
		Size: 4.9 KB (4920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d226da7be978e457796e2e372bc77f0e9a44ccb95bbaba2c0bf7c610d845d349`  
		Last Modified: Wed, 11 Nov 2020 21:50:17 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:c0d2012709484678c0d1aa5ac0e0e46debe0591ddd0a4dedcbb85066702db649
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:8ba28db6cdc5f87b59e4be6c5724d26a11af70b62134f7142b4ef9fd382ef946
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123571140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b89851205aa235471ff68c8daf0701fae60ecb17c385246699e51f5c0eed3ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:18:48 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 25 Nov 2020 23:18:49 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 25 Nov 2020 23:18:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:19:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:19:21 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:19:21 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:19:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 25 Nov 2020 23:19:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:19:23 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:19:23 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd7f0f336d95becc54d7a8b9f7228d46f8dece45218d848109e53c68ea5c8d2`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d455564f5ab63825e4ba7bbe83d44d1f6df04ad7ad11685744303f4e2b8a6d1`  
		Last Modified: Wed, 25 Nov 2020 23:23:11 GMT  
		Size: 86.9 MB (86916418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d384b4810a94b2a0ba6992a4c224f8c5840f6228feda6d71d13b636ebfc20f4`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2e7c2c7df1c88aa47353e1f5bbc1ffe7b2464e1df78143f2638a9e3b61a1dd`  
		Last Modified: Wed, 25 Nov 2020 23:22:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c28cf25f78c7bbfa24896ba86309b733e6cfe7bc74da2ea3f2bcce0f82d2dca8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123322814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1338e0ee6f662e7c6c28a442838755c18e112268d2edd888b63c5f5cc8c3d05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:35:44 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 11 Nov 2020 21:41:32 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 11 Nov 2020 21:41:34 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:42:29 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:42:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:42:32 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:42:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:42:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:42:36 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:42:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a8421f1a1c760507f6e74ce9090cf4fc5f02231f8c1e2634466fef53dd87d`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbacf27f433c06bdfc4a670d9dce4f2a90423b22743b0bfc82a4e7c8a1df4755`  
		Last Modified: Wed, 11 Nov 2020 21:46:56 GMT  
		Size: 88.2 MB (88164721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfeb4eae3c084535b956fff6deed5f955143be859f2e0cde0f60fdc995bf21a`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62fa358c0199b25937629991bf28a1bc6136e9f3cdd83ae5ce9845a73a7e6c`  
		Last Modified: Wed, 11 Nov 2020 21:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:f566897a5981e4fac1713f7aeb8c8aeac8cdced021ef4b0bc07988fca2df5e94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135815909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4698c4cc945a17ebad437bccc342fd4d66f31611b2e65be306d4f4beb1c5f3fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:09:21 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 11 Nov 2020 21:24:57 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Wed, 11 Nov 2020 21:25:08 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:31:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:31:41 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:31:47 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:31:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 Nov 2020 21:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:32:11 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:32:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b315cab93312c5208f46751dc1a4a4e8a98a975507780b22f6d62a581ab6c10`  
		Last Modified: Wed, 11 Nov 2020 21:50:18 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7474eb0da552af0997e1190c05abe7cd5e25450835827dc05a9a67e4723a0e`  
		Last Modified: Wed, 11 Nov 2020 21:50:38 GMT  
		Size: 93.3 MB (93342769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732377b864d33f75b094fe90eac7cf17807e1ffe2709b5929237d32e24c2351`  
		Last Modified: Wed, 11 Nov 2020 21:50:18 GMT  
		Size: 4.9 KB (4920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d226da7be978e457796e2e372bc77f0e9a44ccb95bbaba2c0bf7c610d845d349`  
		Last Modified: Wed, 11 Nov 2020 21:50:17 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:a497d4046a9762617f3203c3c42ab06c78f7e4a2663fed9b3e7f205da7b02d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:be0069ebc09c00f5ff0b1900c5df05eb201cc01d3df4ab7828d26d38fae81654
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125585067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a348a04a8159339ed3ca053ea925f854252e6a6c3df6fa82c17625d1026f18b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 25 Nov 2020 23:18:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:18:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:18:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:18:41 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:18:41 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:18:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8690a3260b734a0e2fe29912f283112edfc4aa22a31bf7282282726e993a8cc`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202ba90333a4d33b3cdeeefcac43e219ea015f484b4b92e14f865621128e237`  
		Last Modified: Wed, 25 Nov 2020 23:22:42 GMT  
		Size: 88.9 MB (88930464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f860b4aa6bf9c5c6f3949001e39c976ac2eddf08295ab842bdc34114ac910`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2b3ef213bead7e743f8b4b3b6fa921cbc963b50a0e89629d934d36c5f2cf7db3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125341391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb59cafebcdf0d75c35d5f018b2192f12e489322be0d89f2ad2bad29635950f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:34:48 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:40:12 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:40:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:41:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:41:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:41:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:41:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:41:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4043d13620ba09e5adff91c927c808500013ef40718f9c667fc415edbbb0fc14`  
		Last Modified: Wed, 11 Nov 2020 21:45:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18247d5d96cbb0445be3ca7366b78e3898db90f269e221dc6a352dd26913431`  
		Last Modified: Wed, 11 Nov 2020 21:46:08 GMT  
		Size: 90.2 MB (90183417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189428954a19e532b3b3af8a3e672fc6513780d0adf3d36d9e5f00228dc2ee94`  
		Last Modified: Wed, 11 Nov 2020 21:45:45 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a9703d1360fae84a4ff8df8d073465ddf5c2f5f12bb4aebd813a5cde3237fed7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137899523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87db369b2668d9ef78329de8a3058dec7d07735661d3489ee8caae0906a89275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:02:43 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:18:26 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:18:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:24:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:24:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:24:27 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988eb6532774207788d05dbdf4b3d057780e0ef2fa395bb5badad4085831dba`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b92a77676842ce52974bfdc0b071724e52629f89ece0aea76241e73e5b846d`  
		Last Modified: Wed, 11 Nov 2020 21:49:43 GMT  
		Size: 95.4 MB (95426507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1080dd4f32be8bc637c4fe10ddef90f2dba8cc8466e816c6263e10af214e06e`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.8`

```console
$ docker pull mariadb@sha256:a497d4046a9762617f3203c3c42ab06c78f7e4a2663fed9b3e7f205da7b02d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.8` - linux; amd64

```console
$ docker pull mariadb@sha256:be0069ebc09c00f5ff0b1900c5df05eb201cc01d3df4ab7828d26d38fae81654
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125585067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a348a04a8159339ed3ca053ea925f854252e6a6c3df6fa82c17625d1026f18b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 25 Nov 2020 23:18:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:18:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:18:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:18:41 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:18:41 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:18:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8690a3260b734a0e2fe29912f283112edfc4aa22a31bf7282282726e993a8cc`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202ba90333a4d33b3cdeeefcac43e219ea015f484b4b92e14f865621128e237`  
		Last Modified: Wed, 25 Nov 2020 23:22:42 GMT  
		Size: 88.9 MB (88930464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f860b4aa6bf9c5c6f3949001e39c976ac2eddf08295ab842bdc34114ac910`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2b3ef213bead7e743f8b4b3b6fa921cbc963b50a0e89629d934d36c5f2cf7db3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125341391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb59cafebcdf0d75c35d5f018b2192f12e489322be0d89f2ad2bad29635950f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:34:48 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:40:12 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:40:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:41:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:41:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:41:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:41:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:41:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4043d13620ba09e5adff91c927c808500013ef40718f9c667fc415edbbb0fc14`  
		Last Modified: Wed, 11 Nov 2020 21:45:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18247d5d96cbb0445be3ca7366b78e3898db90f269e221dc6a352dd26913431`  
		Last Modified: Wed, 11 Nov 2020 21:46:08 GMT  
		Size: 90.2 MB (90183417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189428954a19e532b3b3af8a3e672fc6513780d0adf3d36d9e5f00228dc2ee94`  
		Last Modified: Wed, 11 Nov 2020 21:45:45 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.8` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a9703d1360fae84a4ff8df8d073465ddf5c2f5f12bb4aebd813a5cde3237fed7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137899523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87db369b2668d9ef78329de8a3058dec7d07735661d3489ee8caae0906a89275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:02:43 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:18:26 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:18:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:24:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:24:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:24:27 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988eb6532774207788d05dbdf4b3d057780e0ef2fa395bb5badad4085831dba`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b92a77676842ce52974bfdc0b071724e52629f89ece0aea76241e73e5b846d`  
		Last Modified: Wed, 11 Nov 2020 21:49:43 GMT  
		Size: 95.4 MB (95426507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1080dd4f32be8bc637c4fe10ddef90f2dba8cc8466e816c6263e10af214e06e`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.8-focal`

```console
$ docker pull mariadb@sha256:a497d4046a9762617f3203c3c42ab06c78f7e4a2663fed9b3e7f205da7b02d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.8-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:be0069ebc09c00f5ff0b1900c5df05eb201cc01d3df4ab7828d26d38fae81654
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125585067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a348a04a8159339ed3ca053ea925f854252e6a6c3df6fa82c17625d1026f18b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 25 Nov 2020 23:18:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:18:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:18:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:18:41 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:18:41 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:18:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8690a3260b734a0e2fe29912f283112edfc4aa22a31bf7282282726e993a8cc`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202ba90333a4d33b3cdeeefcac43e219ea015f484b4b92e14f865621128e237`  
		Last Modified: Wed, 25 Nov 2020 23:22:42 GMT  
		Size: 88.9 MB (88930464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f860b4aa6bf9c5c6f3949001e39c976ac2eddf08295ab842bdc34114ac910`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.8-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2b3ef213bead7e743f8b4b3b6fa921cbc963b50a0e89629d934d36c5f2cf7db3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125341391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb59cafebcdf0d75c35d5f018b2192f12e489322be0d89f2ad2bad29635950f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:34:48 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:40:12 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:40:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:41:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:41:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:41:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:41:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:41:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4043d13620ba09e5adff91c927c808500013ef40718f9c667fc415edbbb0fc14`  
		Last Modified: Wed, 11 Nov 2020 21:45:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18247d5d96cbb0445be3ca7366b78e3898db90f269e221dc6a352dd26913431`  
		Last Modified: Wed, 11 Nov 2020 21:46:08 GMT  
		Size: 90.2 MB (90183417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189428954a19e532b3b3af8a3e672fc6513780d0adf3d36d9e5f00228dc2ee94`  
		Last Modified: Wed, 11 Nov 2020 21:45:45 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.8-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a9703d1360fae84a4ff8df8d073465ddf5c2f5f12bb4aebd813a5cde3237fed7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137899523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87db369b2668d9ef78329de8a3058dec7d07735661d3489ee8caae0906a89275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:02:43 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:18:26 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:18:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:24:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:24:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:24:27 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988eb6532774207788d05dbdf4b3d057780e0ef2fa395bb5badad4085831dba`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b92a77676842ce52974bfdc0b071724e52629f89ece0aea76241e73e5b846d`  
		Last Modified: Wed, 11 Nov 2020 21:49:43 GMT  
		Size: 95.4 MB (95426507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1080dd4f32be8bc637c4fe10ddef90f2dba8cc8466e816c6263e10af214e06e`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:a497d4046a9762617f3203c3c42ab06c78f7e4a2663fed9b3e7f205da7b02d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:be0069ebc09c00f5ff0b1900c5df05eb201cc01d3df4ab7828d26d38fae81654
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125585067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a348a04a8159339ed3ca053ea925f854252e6a6c3df6fa82c17625d1026f18b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 25 Nov 2020 23:18:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:18:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:18:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:18:41 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:18:41 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:18:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8690a3260b734a0e2fe29912f283112edfc4aa22a31bf7282282726e993a8cc`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202ba90333a4d33b3cdeeefcac43e219ea015f484b4b92e14f865621128e237`  
		Last Modified: Wed, 25 Nov 2020 23:22:42 GMT  
		Size: 88.9 MB (88930464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f860b4aa6bf9c5c6f3949001e39c976ac2eddf08295ab842bdc34114ac910`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2b3ef213bead7e743f8b4b3b6fa921cbc963b50a0e89629d934d36c5f2cf7db3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125341391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb59cafebcdf0d75c35d5f018b2192f12e489322be0d89f2ad2bad29635950f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:34:48 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:40:12 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:40:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:41:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:41:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:41:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:41:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:41:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4043d13620ba09e5adff91c927c808500013ef40718f9c667fc415edbbb0fc14`  
		Last Modified: Wed, 11 Nov 2020 21:45:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18247d5d96cbb0445be3ca7366b78e3898db90f269e221dc6a352dd26913431`  
		Last Modified: Wed, 11 Nov 2020 21:46:08 GMT  
		Size: 90.2 MB (90183417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189428954a19e532b3b3af8a3e672fc6513780d0adf3d36d9e5f00228dc2ee94`  
		Last Modified: Wed, 11 Nov 2020 21:45:45 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a9703d1360fae84a4ff8df8d073465ddf5c2f5f12bb4aebd813a5cde3237fed7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137899523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87db369b2668d9ef78329de8a3058dec7d07735661d3489ee8caae0906a89275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:02:43 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:18:26 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:18:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:24:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:24:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:24:27 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988eb6532774207788d05dbdf4b3d057780e0ef2fa395bb5badad4085831dba`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b92a77676842ce52974bfdc0b071724e52629f89ece0aea76241e73e5b846d`  
		Last Modified: Wed, 11 Nov 2020 21:49:43 GMT  
		Size: 95.4 MB (95426507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1080dd4f32be8bc637c4fe10ddef90f2dba8cc8466e816c6263e10af214e06e`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:a497d4046a9762617f3203c3c42ab06c78f7e4a2663fed9b3e7f205da7b02d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:be0069ebc09c00f5ff0b1900c5df05eb201cc01d3df4ab7828d26d38fae81654
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125585067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a348a04a8159339ed3ca053ea925f854252e6a6c3df6fa82c17625d1026f18b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 25 Nov 2020 23:18:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:18:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:18:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:18:41 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:18:41 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:18:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8690a3260b734a0e2fe29912f283112edfc4aa22a31bf7282282726e993a8cc`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202ba90333a4d33b3cdeeefcac43e219ea015f484b4b92e14f865621128e237`  
		Last Modified: Wed, 25 Nov 2020 23:22:42 GMT  
		Size: 88.9 MB (88930464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f860b4aa6bf9c5c6f3949001e39c976ac2eddf08295ab842bdc34114ac910`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2b3ef213bead7e743f8b4b3b6fa921cbc963b50a0e89629d934d36c5f2cf7db3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125341391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb59cafebcdf0d75c35d5f018b2192f12e489322be0d89f2ad2bad29635950f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:34:48 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:40:12 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:40:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:41:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:41:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:41:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:41:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:41:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4043d13620ba09e5adff91c927c808500013ef40718f9c667fc415edbbb0fc14`  
		Last Modified: Wed, 11 Nov 2020 21:45:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18247d5d96cbb0445be3ca7366b78e3898db90f269e221dc6a352dd26913431`  
		Last Modified: Wed, 11 Nov 2020 21:46:08 GMT  
		Size: 90.2 MB (90183417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189428954a19e532b3b3af8a3e672fc6513780d0adf3d36d9e5f00228dc2ee94`  
		Last Modified: Wed, 11 Nov 2020 21:45:45 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a9703d1360fae84a4ff8df8d073465ddf5c2f5f12bb4aebd813a5cde3237fed7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137899523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87db369b2668d9ef78329de8a3058dec7d07735661d3489ee8caae0906a89275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:02:43 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:18:26 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:18:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:24:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:24:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:24:27 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988eb6532774207788d05dbdf4b3d057780e0ef2fa395bb5badad4085831dba`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b92a77676842ce52974bfdc0b071724e52629f89ece0aea76241e73e5b846d`  
		Last Modified: Wed, 11 Nov 2020 21:49:43 GMT  
		Size: 95.4 MB (95426507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1080dd4f32be8bc637c4fe10ddef90f2dba8cc8466e816c6263e10af214e06e`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:a497d4046a9762617f3203c3c42ab06c78f7e4a2663fed9b3e7f205da7b02d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:be0069ebc09c00f5ff0b1900c5df05eb201cc01d3df4ab7828d26d38fae81654
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125585067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a348a04a8159339ed3ca053ea925f854252e6a6c3df6fa82c17625d1026f18b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 25 Nov 2020 23:18:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:18:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:18:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:18:41 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:18:41 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:18:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8690a3260b734a0e2fe29912f283112edfc4aa22a31bf7282282726e993a8cc`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202ba90333a4d33b3cdeeefcac43e219ea015f484b4b92e14f865621128e237`  
		Last Modified: Wed, 25 Nov 2020 23:22:42 GMT  
		Size: 88.9 MB (88930464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f860b4aa6bf9c5c6f3949001e39c976ac2eddf08295ab842bdc34114ac910`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2b3ef213bead7e743f8b4b3b6fa921cbc963b50a0e89629d934d36c5f2cf7db3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125341391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb59cafebcdf0d75c35d5f018b2192f12e489322be0d89f2ad2bad29635950f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:34:48 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:40:12 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:40:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:41:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:41:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:41:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:41:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:41:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4043d13620ba09e5adff91c927c808500013ef40718f9c667fc415edbbb0fc14`  
		Last Modified: Wed, 11 Nov 2020 21:45:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18247d5d96cbb0445be3ca7366b78e3898db90f269e221dc6a352dd26913431`  
		Last Modified: Wed, 11 Nov 2020 21:46:08 GMT  
		Size: 90.2 MB (90183417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189428954a19e532b3b3af8a3e672fc6513780d0adf3d36d9e5f00228dc2ee94`  
		Last Modified: Wed, 11 Nov 2020 21:45:45 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a9703d1360fae84a4ff8df8d073465ddf5c2f5f12bb4aebd813a5cde3237fed7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137899523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87db369b2668d9ef78329de8a3058dec7d07735661d3489ee8caae0906a89275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:02:43 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:18:26 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:18:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:24:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:24:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:24:27 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988eb6532774207788d05dbdf4b3d057780e0ef2fa395bb5badad4085831dba`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b92a77676842ce52974bfdc0b071724e52629f89ece0aea76241e73e5b846d`  
		Last Modified: Wed, 11 Nov 2020 21:49:43 GMT  
		Size: 95.4 MB (95426507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1080dd4f32be8bc637c4fe10ddef90f2dba8cc8466e816c6263e10af214e06e`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:a497d4046a9762617f3203c3c42ab06c78f7e4a2663fed9b3e7f205da7b02d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:be0069ebc09c00f5ff0b1900c5df05eb201cc01d3df4ab7828d26d38fae81654
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125585067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a348a04a8159339ed3ca053ea925f854252e6a6c3df6fa82c17625d1026f18b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:26 GMT
ADD file:4f15c4475fbafb3fe335e415e3ea1ac416c34af911fcdfe273c5759438aa8eb4 in / 
# Wed, 25 Nov 2020 22:25:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:17:18 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 25 Nov 2020 23:17:30 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:17:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:17:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:17:55 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 25 Nov 2020 23:17:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 25 Nov 2020 23:17:58 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 25 Nov 2020 23:18:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 25 Nov 2020 23:18:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 25 Nov 2020 23:18:40 GMT
VOLUME [/var/lib/mysql]
# Wed, 25 Nov 2020 23:18:41 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 25 Nov 2020 23:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:18:41 GMT
EXPOSE 3306
# Wed, 25 Nov 2020 23:18:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:da7391352a9bb76b292a568c066aa4c3cbae8d494e6a3c68e3c596d34f7c75f8`  
		Last Modified: Fri, 06 Nov 2020 15:20:07 GMT  
		Size: 28.6 MB (28563271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14428a6d4bcdba49a64127900a0691fb00a3f329aced25eb77e3b65646638f8d`  
		Last Modified: Wed, 25 Nov 2020 22:26:39 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d948710f21ad82dce71743b1654b45acb5c059cf5c19da491582cef6f2601`  
		Last Modified: Wed, 25 Nov 2020 22:26:40 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22776aa82430af24b71cc0294b9c2bddd7c9f4a0213d13967e3bccc4f1296948`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e64230d63d996dc81a927a75ec71730d7bb1ece4e43d64d6f2b830dab4bc82`  
		Last Modified: Wed, 25 Nov 2020 23:22:28 GMT  
		Size: 5.5 MB (5488627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30861f14a103eb6617d70c0b3ddb21d08ac133ed9d4e073f16e6b17a089d539`  
		Last Modified: Wed, 25 Nov 2020 23:22:26 GMT  
		Size: 1.3 MB (1324655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e9e6a3da2446ca697e0ccb0d7c44012e8573d4eb708b36f11a876657970d7b`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420a23f08c4147516e0f33d70c17c7f4d7a1e1ae4db8deb2a6a703f2c565483a`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 1.3 MB (1267437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd73f23de4821d5ddc74bdc29ed54ccafac21587e18baf11431413d7906c4371`  
		Last Modified: Wed, 25 Nov 2020 23:22:25 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8690a3260b734a0e2fe29912f283112edfc4aa22a31bf7282282726e993a8cc`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202ba90333a4d33b3cdeeefcac43e219ea015f484b4b92e14f865621128e237`  
		Last Modified: Wed, 25 Nov 2020 23:22:42 GMT  
		Size: 88.9 MB (88930464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f860b4aa6bf9c5c6f3949001e39c976ac2eddf08295ab842bdc34114ac910`  
		Last Modified: Wed, 25 Nov 2020 23:22:24 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:2b3ef213bead7e743f8b4b3b6fa921cbc963b50a0e89629d934d36c5f2cf7db3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125341391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb59cafebcdf0d75c35d5f018b2192f12e489322be0d89f2ad2bad29635950f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 18:19:38 GMT
ADD file:83fb716eb29f83f9e0ea0422f76e651689972d98764d3e19e4017bbd3fe9d6e4 in / 
# Fri, 23 Oct 2020 18:19:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 18:19:42 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 18:19:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 18:19:45 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:33:56 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:34:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:14 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 19:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 19:34:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 19:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:34:45 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 19:34:47 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 19:34:48 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:40:12 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:40:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:41:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:41:09 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:41:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:41:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:41:13 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:41:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:00f57adb053c38c53d0655dee1ba47ed4cbd78cade062cf0e00f4b9790c7ed36`  
		Last Modified: Thu, 08 Oct 2020 08:25:26 GMT  
		Size: 27.2 MB (27163834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235828e8d75b4f9129ec8b0a00d4e3f1c4d100eedb3f00696a2ec78862082f6`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b606b1b8abdd386d8de6d1ce374b4dcdd4f7bcb4d68db64f09c03520fa5bf5`  
		Last Modified: Fri, 23 Oct 2020 18:20:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1c04936d96ea5c0317454491309061a9bbb71f304201beba9d2a84d70278c6`  
		Last Modified: Fri, 23 Oct 2020 19:38:48 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838094e6dc11e995240cf827f8ba4add82c55538799aa31d59b62833848b4a7f`  
		Last Modified: Fri, 23 Oct 2020 19:38:49 GMT  
		Size: 5.5 MB (5456163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156fbd7c528b7c56c7aab3103cd246779fc21c2d0704f38d68cf9e0e24ce0ec`  
		Last Modified: Fri, 23 Oct 2020 19:38:47 GMT  
		Size: 1.3 MB (1261580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96338e63cb2211929a174adb8f3717e1a2a8819e52367fcca58513ccb068d867`  
		Last Modified: Fri, 23 Oct 2020 19:38:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072483a93c1f4fdd36a34d7ec0087b270002ffc4b396eb10a969609ed1364d58`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 1.3 MB (1265714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708913510fbcb15b1b99d5e6f4069454c58d03a3065c6bc95bb8ab01af8390a5`  
		Last Modified: Fri, 23 Oct 2020 19:38:45 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4043d13620ba09e5adff91c927c808500013ef40718f9c667fc415edbbb0fc14`  
		Last Modified: Wed, 11 Nov 2020 21:45:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18247d5d96cbb0445be3ca7366b78e3898db90f269e221dc6a352dd26913431`  
		Last Modified: Wed, 11 Nov 2020 21:46:08 GMT  
		Size: 90.2 MB (90183417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189428954a19e532b3b3af8a3e672fc6513780d0adf3d36d9e5f00228dc2ee94`  
		Last Modified: Wed, 11 Nov 2020 21:45:45 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a9703d1360fae84a4ff8df8d073465ddf5c2f5f12bb4aebd813a5cde3237fed7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137899523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87db369b2668d9ef78329de8a3058dec7d07735661d3489ee8caae0906a89275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 23 Oct 2020 19:25:52 GMT
ADD file:b9c09681764b8697badc8139e82a30efeb353faf61258695d1cd3a843c4de6a8 in / 
# Fri, 23 Oct 2020 19:26:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 19:26:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 19:26:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 19:27:03 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 19:55:22 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 23 Oct 2020 19:58:32 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 19:58:41 GMT
ENV GOSU_VERSION=1.12
# Fri, 23 Oct 2020 20:00:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 23 Oct 2020 20:01:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 23 Oct 2020 20:01:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 20:02:11 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 23 Oct 2020 20:02:36 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 23 Oct 2020 20:02:43 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 11 Nov 2020 21:18:26 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Wed, 11 Nov 2020 21:18:33 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 11 Nov 2020 21:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 11 Nov 2020 21:24:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 Nov 2020 21:24:19 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Wed, 11 Nov 2020 21:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Nov 2020 21:24:27 GMT
EXPOSE 3306
# Wed, 11 Nov 2020 21:24:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:76ff736f6fb2d41940a6cbdeab4242e9a64ef7df99ee4f3d9fcb9ec67bfccfc6`  
		Last Modified: Mon, 12 Oct 2020 16:20:28 GMT  
		Size: 33.3 MB (33275528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d354673d1251716a1ed9cc3460095ee31664859e23d7e616546a17d287728`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434fabf01a92cfd54e3ae6f5e3dc7a3837ac2199999f713fbdf5cb2c800324a2`  
		Last Modified: Fri, 23 Oct 2020 19:31:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8d4d42dc304605f1e3308df16201cafdb993d4a53eb11c8865e444f603c85`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86154d9082951c9b2d658939cd2ebb2acd95a4609822131d650df7c34b26de8d`  
		Last Modified: Fri, 23 Oct 2020 20:26:26 GMT  
		Size: 6.7 MB (6668872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4317eb498e78b7b1ab9b98604730dd23addd5877207fee2e29065cc2a597519`  
		Last Modified: Fri, 23 Oct 2020 20:26:27 GMT  
		Size: 1.2 MB (1244112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ee0bfbaadf08c70669d0ad3554b95a987af156889225eb5d82186c4aed3870`  
		Last Modified: Fri, 23 Oct 2020 20:26:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417da7e19201985162a4accf079629ab39a993d10ef41725c420a47557f878b`  
		Last Modified: Fri, 23 Oct 2020 20:26:20 GMT  
		Size: 1.3 MB (1273805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a761192d0ae5dd38ad710f39b7965f2ddf2f289179c0643f1500ed08367122`  
		Last Modified: Fri, 23 Oct 2020 20:26:18 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0988eb6532774207788d05dbdf4b3d057780e0ef2fa395bb5badad4085831dba`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b92a77676842ce52974bfdc0b071724e52629f89ece0aea76241e73e5b846d`  
		Last Modified: Wed, 11 Nov 2020 21:49:43 GMT  
		Size: 95.4 MB (95426507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1080dd4f32be8bc637c4fe10ddef90f2dba8cc8466e816c6263e10af214e06e`  
		Last Modified: Wed, 11 Nov 2020 21:49:22 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
