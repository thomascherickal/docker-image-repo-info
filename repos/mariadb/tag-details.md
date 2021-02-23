<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10.1`](#mariadb101)
-	[`mariadb:10.1.48`](#mariadb10148)
-	[`mariadb:10.1.48-bionic`](#mariadb10148-bionic)
-	[`mariadb:10.1-bionic`](#mariadb101-bionic)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2.37`](#mariadb10237)
-	[`mariadb:10.2.37-bionic`](#mariadb10237-bionic)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3.28`](#mariadb10328)
-	[`mariadb:10.3.28-focal`](#mariadb10328-focal)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4.18`](#mariadb10418)
-	[`mariadb:10.4.18-focal`](#mariadb10418-focal)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5.9`](#mariadb1059)
-	[`mariadb:10.5.9-focal`](#mariadb1059-focal)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:a13b01d9af44097efeca7a3808a524c8052870e59a1eeef074857ba01e70c1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:d866e756c68fce525419ee27e1d76a874c54072e49dfd591891acd28f95760fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124234067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e69b4a7bda8206563d333112c11de8f043815f996d896afae748c977306746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:22:12 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:22:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:22:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:22:52 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:22:52 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:22:53 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:22:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c59f9e205048d588bf0348ecfadb4ae9c1129ba81f8aedf720fd3446408ff`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa441240c225aa867489089e770da81a847b66e18c1cf5bddb79f7e2c8400e4`  
		Last Modified: Mon, 22 Feb 2021 23:25:57 GMT  
		Size: 87.6 MB (87572628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fee6e1dead96fa856d7afa714bd0d4f2eacb5e3822ea519890a7084837be52`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:eacab2a85f2692a71bbecec0ec1d4eab0a813409bc4760b2d15269b05aa2bafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121825675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d6819532a366f80a8a12c2f9e4ba95c2de67748fce8fc06ce32c95095f896d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:40:27 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 22:56:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 22:56:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:57:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:57:40 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:57:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:57:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:57:42 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:57:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29485c9b3cd7eb629c66e8b4a0c8fb3ebb2aa9d2e840e03c64e50087e27ae68`  
		Last Modified: Mon, 22 Feb 2021 23:02:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73aa765ec3b0d56d75bf82710cf3630aeb5f2d43d953ee4e846a3e729d5360`  
		Last Modified: Mon, 22 Feb 2021 23:02:32 GMT  
		Size: 86.7 MB (86652702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e7e791fe18cdc43a40a9a092228efabefe76675de202cbb4a11810b9a452f5`  
		Last Modified: Mon, 22 Feb 2021 23:02:09 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:579b94998b567c524563c8eb2ce1a995f626c363c4ebcce4e0f76c6ebeb4d433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e61642b22fa5ad1b5375824f6906cb9be6ed44ce44598c8c38a76ad7547341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:40 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:16:43 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:16:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:26:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:26:37 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:26:41 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:26:58 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9408f76f8efc8cd4e636b1149ae5c0000b07e0c008aef9453414b7467eb3886`  
		Last Modified: Mon, 22 Feb 2021 23:47:40 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e97e4b9d88b8ee80ced97b5cd60b0e70dfa733e30f855d2395cc43295224fe`  
		Last Modified: Mon, 22 Feb 2021 23:48:00 GMT  
		Size: 92.2 MB (92197515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f1911e37adab2eb549dd7070427a998202609efd248bb17eb0118a0ae2132c`  
		Last Modified: Mon, 22 Feb 2021 23:47:39 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1`

```console
$ docker pull mariadb@sha256:6a101313d6ed41c32e18defeafb2119439c3dfa2906c094b8adc0f54f9c6c762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1` - linux; amd64

```console
$ docker pull mariadb@sha256:c0900ba3a5c89830306956a5972cf598b33dd43955de1d448dca4a349beb35f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113175266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005b719edf129131224e961950e4ae05c47611c28713e3889fcba82df4e27ace`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 12:00:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 12:00:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:23 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 12:00:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 12:00:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 12:00:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 12:00:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 12:01:34 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 12:01:34 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 12:01:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 12:02:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 12:02:15 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:25:14 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:25:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:25:15 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:25:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e1d55d7187e8f362e53e468bc013ece20d08729dfa19233d4b201ea6c0fdd`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbd8eb6c494fbc05415014eca7a11f912cb7a6db85b18e0251e25aedb0f1cf`  
		Last Modified: Thu, 21 Jan 2021 12:04:31 GMT  
		Size: 4.8 MB (4811143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba484d25fdf813b30ca6199138092b8ed6ffa98bb5e742ad0d79e7057203632c`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.3 MB (1326584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3721839f3a0dcdcf6255072f1782da13e42a4068eb1eba2ec8fa8fd589289be`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0624c9c3aad26b62edc6088904a5782131a5b527711d3a6ac7ad4d663e492b83`  
		Last Modified: Thu, 21 Jan 2021 12:04:28 GMT  
		Size: 932.3 KB (932287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0756263074505a61315650e925f2530ee01ad1ea54bbd5cee32a20dc5b540973`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69098fc756115c84ae1a0b2c1dc68975c1aa0fd11a073c119530933391f4b732`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7243881889c21aa98065ca3023b18091a5ea8940e200ee52c104df345cf2b5`  
		Last Modified: Thu, 21 Jan 2021 12:05:05 GMT  
		Size: 79.4 MB (79381883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8634d847d477aff610c669ae7a55524ab5c7271a71ed048c3c15fcffa7dc7686`  
		Last Modified: Mon, 22 Feb 2021 23:27:20 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d201307e5c66c5f6a23421cb046d2614198a017faf3755bf2873cc48bdd56c8`  
		Last Modified: Mon, 22 Feb 2021 23:27:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:62774c810f99a0aa8475c01c39e2d89d24e4bebfb1107cf9ef5486022c4a19e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105800468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c1aa6a77140ec33512e8ca7e69ad6ce576724194dfdcec5e8d642019faadcd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:43:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:43:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:43:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:44:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:44:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:44:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:44:21 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:44:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:45:32 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 05:45:33 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 05:45:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:46:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:46:22 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:01:37 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:01:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:01:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:01:41 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:01:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0913f7e8916a73df7595a8eed8504a0fe2b9a1ef0eb726442f2d3ddd62e6c29f`  
		Last Modified: Thu, 21 Jan 2021 05:49:13 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e8c54ecac617f1826858c0e6ca4c741eaa268f514e5bc12a9b9ff403c8c97c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 4.4 MB (4394730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de0e92bd62367167d5ecb0e93306cb8f77e9eda05a006fab36ad7843c3e06f`  
		Last Modified: Thu, 21 Jan 2021 05:49:10 GMT  
		Size: 1.3 MB (1263716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0265c953d9ee94de17c5d84e00c0dea2c5b71a1d022ecce588eae2d642ad5c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d8e12d2b1bb184b49dce9c2717a0adb1dca18e8c5f65ae57867ae5e8987b7`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 925.3 KB (925349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4a1e7930ee33a2c49dea2d0899a87a3f76ad932ba63f9ad479372bd8bab97`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67f577c7f1b024005d873246f67ef9b229780ae53549e6f452fa80a43facfb1`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b8c3335e4b210ef60e457cd66835e85073d1941dfa65e26df5d7ccb9f7ef31`  
		Last Modified: Thu, 21 Jan 2021 05:50:04 GMT  
		Size: 75.5 MB (75470315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8982517ef9259ee7ca0bcd24069e5b20fc043df6e1808db05c047a30fe1c99fc`  
		Last Modified: Mon, 22 Feb 2021 23:04:32 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03acfc19adda6e0aaa1c74327fca8ebddb0cf92f504039465e87d72a2b62548f`  
		Last Modified: Mon, 22 Feb 2021 23:04:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; ppc64le

```console
$ docker pull mariadb@sha256:de83b01fa8656bb1c3e2e9874c307a51cc3cd01fa566075a1a770e75a4ebc050
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c3753ffb7b3d0cae21757780a52abf16ec517df24cea4243f40519384b3bcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:03 GMT
ADD file:f6214eb5991df55aa5198d84442d6ddd28b67d4043d1832afba8b30e0249dcf5 in / 
# Thu, 21 Jan 2021 03:49:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:08:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 06:10:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:10:45 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 06:11:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 06:12:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 06:12:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:12:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 06:12:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:17:55 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 06:18:01 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 06:18:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:22:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:22:16 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:46:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:46:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:46:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:46:55 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:47:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e07786faec2ce77c08f20befe52a3eac52d983b0dfae9cb8d58dfa0ede0648e1`  
		Last Modified: Thu, 21 Jan 2021 03:54:37 GMT  
		Size: 30.4 MB (30422854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a41aaf71d5cf82fa1f9e11d2d352906ae135d0b216c665ed76ad9a8e1ce046`  
		Last Modified: Thu, 21 Jan 2021 03:54:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e417a2309160c84b59c2e2ca585c0c1bd11a20876b7b04f00ed626592cc50e3`  
		Last Modified: Thu, 21 Jan 2021 06:29:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902524cdd9e3f0443a75babb289e129c0c2ec2b986161aa293ea8100cc77242b`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 5.6 MB (5630103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e198886a17e45226cfc6e3993ef55ca78556f6668984578c614bb01f0842e46`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 1.2 MB (1246925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953fb576afa139daf106d7a5511866370880e5a9b887ee386312bf0fcdd74d0`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d19ff23593668af110ba0e7d4a012fed889478daa306ab627946ff849286d5`  
		Last Modified: Thu, 21 Jan 2021 06:29:24 GMT  
		Size: 934.8 KB (934827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08451c7ddd7e19ffd1ed4c579ab92382506bedd27f02d3a0a9a481ef37b30887`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7b841158ff59be5418005816766fb3a79d97b14481688aad52d195b00fb654`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0e773762e9e799e50a66a4f5c9757ab1b9c3e22642ce1a349d9e0bccf1ebcd`  
		Last Modified: Thu, 21 Jan 2021 06:30:17 GMT  
		Size: 79.9 MB (79924102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8607404c5be8478cbb432cdcae5b24aaaebf1f59c54fcae6ffa9d685b0901c28`  
		Last Modified: Mon, 22 Feb 2021 23:50:20 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57907cace02e5b37ca3cb19bbd04bc9653b7980fbd1a53faa2f4ef9416a0302f`  
		Last Modified: Mon, 22 Feb 2021 23:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48`

```console
$ docker pull mariadb@sha256:6a101313d6ed41c32e18defeafb2119439c3dfa2906c094b8adc0f54f9c6c762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48` - linux; amd64

```console
$ docker pull mariadb@sha256:c0900ba3a5c89830306956a5972cf598b33dd43955de1d448dca4a349beb35f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113175266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005b719edf129131224e961950e4ae05c47611c28713e3889fcba82df4e27ace`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 12:00:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 12:00:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:23 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 12:00:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 12:00:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 12:00:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 12:00:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 12:01:34 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 12:01:34 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 12:01:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 12:02:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 12:02:15 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:25:14 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:25:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:25:15 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:25:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e1d55d7187e8f362e53e468bc013ece20d08729dfa19233d4b201ea6c0fdd`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbd8eb6c494fbc05415014eca7a11f912cb7a6db85b18e0251e25aedb0f1cf`  
		Last Modified: Thu, 21 Jan 2021 12:04:31 GMT  
		Size: 4.8 MB (4811143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba484d25fdf813b30ca6199138092b8ed6ffa98bb5e742ad0d79e7057203632c`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.3 MB (1326584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3721839f3a0dcdcf6255072f1782da13e42a4068eb1eba2ec8fa8fd589289be`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0624c9c3aad26b62edc6088904a5782131a5b527711d3a6ac7ad4d663e492b83`  
		Last Modified: Thu, 21 Jan 2021 12:04:28 GMT  
		Size: 932.3 KB (932287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0756263074505a61315650e925f2530ee01ad1ea54bbd5cee32a20dc5b540973`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69098fc756115c84ae1a0b2c1dc68975c1aa0fd11a073c119530933391f4b732`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7243881889c21aa98065ca3023b18091a5ea8940e200ee52c104df345cf2b5`  
		Last Modified: Thu, 21 Jan 2021 12:05:05 GMT  
		Size: 79.4 MB (79381883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8634d847d477aff610c669ae7a55524ab5c7271a71ed048c3c15fcffa7dc7686`  
		Last Modified: Mon, 22 Feb 2021 23:27:20 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d201307e5c66c5f6a23421cb046d2614198a017faf3755bf2873cc48bdd56c8`  
		Last Modified: Mon, 22 Feb 2021 23:27:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:62774c810f99a0aa8475c01c39e2d89d24e4bebfb1107cf9ef5486022c4a19e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105800468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c1aa6a77140ec33512e8ca7e69ad6ce576724194dfdcec5e8d642019faadcd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:43:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:43:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:43:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:44:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:44:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:44:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:44:21 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:44:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:45:32 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 05:45:33 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 05:45:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:46:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:46:22 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:01:37 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:01:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:01:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:01:41 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:01:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0913f7e8916a73df7595a8eed8504a0fe2b9a1ef0eb726442f2d3ddd62e6c29f`  
		Last Modified: Thu, 21 Jan 2021 05:49:13 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e8c54ecac617f1826858c0e6ca4c741eaa268f514e5bc12a9b9ff403c8c97c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 4.4 MB (4394730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de0e92bd62367167d5ecb0e93306cb8f77e9eda05a006fab36ad7843c3e06f`  
		Last Modified: Thu, 21 Jan 2021 05:49:10 GMT  
		Size: 1.3 MB (1263716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0265c953d9ee94de17c5d84e00c0dea2c5b71a1d022ecce588eae2d642ad5c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d8e12d2b1bb184b49dce9c2717a0adb1dca18e8c5f65ae57867ae5e8987b7`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 925.3 KB (925349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4a1e7930ee33a2c49dea2d0899a87a3f76ad932ba63f9ad479372bd8bab97`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67f577c7f1b024005d873246f67ef9b229780ae53549e6f452fa80a43facfb1`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b8c3335e4b210ef60e457cd66835e85073d1941dfa65e26df5d7ccb9f7ef31`  
		Last Modified: Thu, 21 Jan 2021 05:50:04 GMT  
		Size: 75.5 MB (75470315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8982517ef9259ee7ca0bcd24069e5b20fc043df6e1808db05c047a30fe1c99fc`  
		Last Modified: Mon, 22 Feb 2021 23:04:32 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03acfc19adda6e0aaa1c74327fca8ebddb0cf92f504039465e87d72a2b62548f`  
		Last Modified: Mon, 22 Feb 2021 23:04:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; ppc64le

```console
$ docker pull mariadb@sha256:de83b01fa8656bb1c3e2e9874c307a51cc3cd01fa566075a1a770e75a4ebc050
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c3753ffb7b3d0cae21757780a52abf16ec517df24cea4243f40519384b3bcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:03 GMT
ADD file:f6214eb5991df55aa5198d84442d6ddd28b67d4043d1832afba8b30e0249dcf5 in / 
# Thu, 21 Jan 2021 03:49:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:08:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 06:10:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:10:45 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 06:11:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 06:12:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 06:12:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:12:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 06:12:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:17:55 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 06:18:01 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 06:18:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:22:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:22:16 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:46:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:46:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:46:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:46:55 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:47:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e07786faec2ce77c08f20befe52a3eac52d983b0dfae9cb8d58dfa0ede0648e1`  
		Last Modified: Thu, 21 Jan 2021 03:54:37 GMT  
		Size: 30.4 MB (30422854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a41aaf71d5cf82fa1f9e11d2d352906ae135d0b216c665ed76ad9a8e1ce046`  
		Last Modified: Thu, 21 Jan 2021 03:54:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e417a2309160c84b59c2e2ca585c0c1bd11a20876b7b04f00ed626592cc50e3`  
		Last Modified: Thu, 21 Jan 2021 06:29:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902524cdd9e3f0443a75babb289e129c0c2ec2b986161aa293ea8100cc77242b`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 5.6 MB (5630103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e198886a17e45226cfc6e3993ef55ca78556f6668984578c614bb01f0842e46`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 1.2 MB (1246925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953fb576afa139daf106d7a5511866370880e5a9b887ee386312bf0fcdd74d0`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d19ff23593668af110ba0e7d4a012fed889478daa306ab627946ff849286d5`  
		Last Modified: Thu, 21 Jan 2021 06:29:24 GMT  
		Size: 934.8 KB (934827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08451c7ddd7e19ffd1ed4c579ab92382506bedd27f02d3a0a9a481ef37b30887`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7b841158ff59be5418005816766fb3a79d97b14481688aad52d195b00fb654`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0e773762e9e799e50a66a4f5c9757ab1b9c3e22642ce1a349d9e0bccf1ebcd`  
		Last Modified: Thu, 21 Jan 2021 06:30:17 GMT  
		Size: 79.9 MB (79924102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8607404c5be8478cbb432cdcae5b24aaaebf1f59c54fcae6ffa9d685b0901c28`  
		Last Modified: Mon, 22 Feb 2021 23:50:20 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57907cace02e5b37ca3cb19bbd04bc9653b7980fbd1a53faa2f4ef9416a0302f`  
		Last Modified: Mon, 22 Feb 2021 23:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48-bionic`

```console
$ docker pull mariadb@sha256:6a101313d6ed41c32e18defeafb2119439c3dfa2906c094b8adc0f54f9c6c762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:c0900ba3a5c89830306956a5972cf598b33dd43955de1d448dca4a349beb35f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113175266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005b719edf129131224e961950e4ae05c47611c28713e3889fcba82df4e27ace`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 12:00:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 12:00:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:23 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 12:00:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 12:00:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 12:00:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 12:00:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 12:01:34 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 12:01:34 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 12:01:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 12:02:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 12:02:15 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:25:14 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:25:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:25:15 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:25:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e1d55d7187e8f362e53e468bc013ece20d08729dfa19233d4b201ea6c0fdd`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbd8eb6c494fbc05415014eca7a11f912cb7a6db85b18e0251e25aedb0f1cf`  
		Last Modified: Thu, 21 Jan 2021 12:04:31 GMT  
		Size: 4.8 MB (4811143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba484d25fdf813b30ca6199138092b8ed6ffa98bb5e742ad0d79e7057203632c`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.3 MB (1326584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3721839f3a0dcdcf6255072f1782da13e42a4068eb1eba2ec8fa8fd589289be`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0624c9c3aad26b62edc6088904a5782131a5b527711d3a6ac7ad4d663e492b83`  
		Last Modified: Thu, 21 Jan 2021 12:04:28 GMT  
		Size: 932.3 KB (932287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0756263074505a61315650e925f2530ee01ad1ea54bbd5cee32a20dc5b540973`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69098fc756115c84ae1a0b2c1dc68975c1aa0fd11a073c119530933391f4b732`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7243881889c21aa98065ca3023b18091a5ea8940e200ee52c104df345cf2b5`  
		Last Modified: Thu, 21 Jan 2021 12:05:05 GMT  
		Size: 79.4 MB (79381883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8634d847d477aff610c669ae7a55524ab5c7271a71ed048c3c15fcffa7dc7686`  
		Last Modified: Mon, 22 Feb 2021 23:27:20 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d201307e5c66c5f6a23421cb046d2614198a017faf3755bf2873cc48bdd56c8`  
		Last Modified: Mon, 22 Feb 2021 23:27:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:62774c810f99a0aa8475c01c39e2d89d24e4bebfb1107cf9ef5486022c4a19e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105800468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c1aa6a77140ec33512e8ca7e69ad6ce576724194dfdcec5e8d642019faadcd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:43:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:43:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:43:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:44:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:44:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:44:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:44:21 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:44:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:45:32 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 05:45:33 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 05:45:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:46:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:46:22 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:01:37 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:01:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:01:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:01:41 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:01:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0913f7e8916a73df7595a8eed8504a0fe2b9a1ef0eb726442f2d3ddd62e6c29f`  
		Last Modified: Thu, 21 Jan 2021 05:49:13 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e8c54ecac617f1826858c0e6ca4c741eaa268f514e5bc12a9b9ff403c8c97c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 4.4 MB (4394730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de0e92bd62367167d5ecb0e93306cb8f77e9eda05a006fab36ad7843c3e06f`  
		Last Modified: Thu, 21 Jan 2021 05:49:10 GMT  
		Size: 1.3 MB (1263716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0265c953d9ee94de17c5d84e00c0dea2c5b71a1d022ecce588eae2d642ad5c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d8e12d2b1bb184b49dce9c2717a0adb1dca18e8c5f65ae57867ae5e8987b7`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 925.3 KB (925349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4a1e7930ee33a2c49dea2d0899a87a3f76ad932ba63f9ad479372bd8bab97`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67f577c7f1b024005d873246f67ef9b229780ae53549e6f452fa80a43facfb1`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b8c3335e4b210ef60e457cd66835e85073d1941dfa65e26df5d7ccb9f7ef31`  
		Last Modified: Thu, 21 Jan 2021 05:50:04 GMT  
		Size: 75.5 MB (75470315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8982517ef9259ee7ca0bcd24069e5b20fc043df6e1808db05c047a30fe1c99fc`  
		Last Modified: Mon, 22 Feb 2021 23:04:32 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03acfc19adda6e0aaa1c74327fca8ebddb0cf92f504039465e87d72a2b62548f`  
		Last Modified: Mon, 22 Feb 2021 23:04:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:de83b01fa8656bb1c3e2e9874c307a51cc3cd01fa566075a1a770e75a4ebc050
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c3753ffb7b3d0cae21757780a52abf16ec517df24cea4243f40519384b3bcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:03 GMT
ADD file:f6214eb5991df55aa5198d84442d6ddd28b67d4043d1832afba8b30e0249dcf5 in / 
# Thu, 21 Jan 2021 03:49:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:08:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 06:10:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:10:45 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 06:11:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 06:12:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 06:12:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:12:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 06:12:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:17:55 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 06:18:01 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 06:18:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:22:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:22:16 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:46:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:46:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:46:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:46:55 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:47:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e07786faec2ce77c08f20befe52a3eac52d983b0dfae9cb8d58dfa0ede0648e1`  
		Last Modified: Thu, 21 Jan 2021 03:54:37 GMT  
		Size: 30.4 MB (30422854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a41aaf71d5cf82fa1f9e11d2d352906ae135d0b216c665ed76ad9a8e1ce046`  
		Last Modified: Thu, 21 Jan 2021 03:54:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e417a2309160c84b59c2e2ca585c0c1bd11a20876b7b04f00ed626592cc50e3`  
		Last Modified: Thu, 21 Jan 2021 06:29:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902524cdd9e3f0443a75babb289e129c0c2ec2b986161aa293ea8100cc77242b`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 5.6 MB (5630103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e198886a17e45226cfc6e3993ef55ca78556f6668984578c614bb01f0842e46`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 1.2 MB (1246925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953fb576afa139daf106d7a5511866370880e5a9b887ee386312bf0fcdd74d0`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d19ff23593668af110ba0e7d4a012fed889478daa306ab627946ff849286d5`  
		Last Modified: Thu, 21 Jan 2021 06:29:24 GMT  
		Size: 934.8 KB (934827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08451c7ddd7e19ffd1ed4c579ab92382506bedd27f02d3a0a9a481ef37b30887`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7b841158ff59be5418005816766fb3a79d97b14481688aad52d195b00fb654`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0e773762e9e799e50a66a4f5c9757ab1b9c3e22642ce1a349d9e0bccf1ebcd`  
		Last Modified: Thu, 21 Jan 2021 06:30:17 GMT  
		Size: 79.9 MB (79924102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8607404c5be8478cbb432cdcae5b24aaaebf1f59c54fcae6ffa9d685b0901c28`  
		Last Modified: Mon, 22 Feb 2021 23:50:20 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57907cace02e5b37ca3cb19bbd04bc9653b7980fbd1a53faa2f4ef9416a0302f`  
		Last Modified: Mon, 22 Feb 2021 23:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1-bionic`

```console
$ docker pull mariadb@sha256:6a101313d6ed41c32e18defeafb2119439c3dfa2906c094b8adc0f54f9c6c762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:c0900ba3a5c89830306956a5972cf598b33dd43955de1d448dca4a349beb35f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113175266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005b719edf129131224e961950e4ae05c47611c28713e3889fcba82df4e27ace`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 12:00:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 12:00:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:23 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 12:00:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 12:00:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 12:00:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 12:00:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 12:01:34 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 12:01:34 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 12:01:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 12:02:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 12:02:15 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:25:14 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:25:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:25:15 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:25:16 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e1d55d7187e8f362e53e468bc013ece20d08729dfa19233d4b201ea6c0fdd`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbd8eb6c494fbc05415014eca7a11f912cb7a6db85b18e0251e25aedb0f1cf`  
		Last Modified: Thu, 21 Jan 2021 12:04:31 GMT  
		Size: 4.8 MB (4811143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba484d25fdf813b30ca6199138092b8ed6ffa98bb5e742ad0d79e7057203632c`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.3 MB (1326584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3721839f3a0dcdcf6255072f1782da13e42a4068eb1eba2ec8fa8fd589289be`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0624c9c3aad26b62edc6088904a5782131a5b527711d3a6ac7ad4d663e492b83`  
		Last Modified: Thu, 21 Jan 2021 12:04:28 GMT  
		Size: 932.3 KB (932287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0756263074505a61315650e925f2530ee01ad1ea54bbd5cee32a20dc5b540973`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69098fc756115c84ae1a0b2c1dc68975c1aa0fd11a073c119530933391f4b732`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7243881889c21aa98065ca3023b18091a5ea8940e200ee52c104df345cf2b5`  
		Last Modified: Thu, 21 Jan 2021 12:05:05 GMT  
		Size: 79.4 MB (79381883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8634d847d477aff610c669ae7a55524ab5c7271a71ed048c3c15fcffa7dc7686`  
		Last Modified: Mon, 22 Feb 2021 23:27:20 GMT  
		Size: 5.0 KB (5030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d201307e5c66c5f6a23421cb046d2614198a017faf3755bf2873cc48bdd56c8`  
		Last Modified: Mon, 22 Feb 2021 23:27:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:62774c810f99a0aa8475c01c39e2d89d24e4bebfb1107cf9ef5486022c4a19e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105800468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c1aa6a77140ec33512e8ca7e69ad6ce576724194dfdcec5e8d642019faadcd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:43:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:43:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:43:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:44:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:44:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:44:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:44:21 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:44:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:45:32 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 05:45:33 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 05:45:35 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:46:20 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:46:22 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:01:37 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:01:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:01:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:01:41 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:01:42 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0913f7e8916a73df7595a8eed8504a0fe2b9a1ef0eb726442f2d3ddd62e6c29f`  
		Last Modified: Thu, 21 Jan 2021 05:49:13 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e8c54ecac617f1826858c0e6ca4c741eaa268f514e5bc12a9b9ff403c8c97c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 4.4 MB (4394730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de0e92bd62367167d5ecb0e93306cb8f77e9eda05a006fab36ad7843c3e06f`  
		Last Modified: Thu, 21 Jan 2021 05:49:10 GMT  
		Size: 1.3 MB (1263716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0265c953d9ee94de17c5d84e00c0dea2c5b71a1d022ecce588eae2d642ad5c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d8e12d2b1bb184b49dce9c2717a0adb1dca18e8c5f65ae57867ae5e8987b7`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 925.3 KB (925349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4a1e7930ee33a2c49dea2d0899a87a3f76ad932ba63f9ad479372bd8bab97`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67f577c7f1b024005d873246f67ef9b229780ae53549e6f452fa80a43facfb1`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b8c3335e4b210ef60e457cd66835e85073d1941dfa65e26df5d7ccb9f7ef31`  
		Last Modified: Thu, 21 Jan 2021 05:50:04 GMT  
		Size: 75.5 MB (75470315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8982517ef9259ee7ca0bcd24069e5b20fc043df6e1808db05c047a30fe1c99fc`  
		Last Modified: Mon, 22 Feb 2021 23:04:32 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03acfc19adda6e0aaa1c74327fca8ebddb0cf92f504039465e87d72a2b62548f`  
		Last Modified: Mon, 22 Feb 2021 23:04:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:de83b01fa8656bb1c3e2e9874c307a51cc3cd01fa566075a1a770e75a4ebc050
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9c3753ffb7b3d0cae21757780a52abf16ec517df24cea4243f40519384b3bcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:03 GMT
ADD file:f6214eb5991df55aa5198d84442d6ddd28b67d4043d1832afba8b30e0249dcf5 in / 
# Thu, 21 Jan 2021 03:49:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:08:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 06:10:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:10:45 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 06:11:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 06:12:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 06:12:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:12:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 06:12:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:17:55 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 21 Jan 2021 06:18:01 GMT
ENV MARIADB_VERSION=1:10.1.48+maria-1~bionic
# Thu, 21 Jan 2021 06:18:22 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:22:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:22:16 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:46:17 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:46:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:46:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:46:55 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:47:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e07786faec2ce77c08f20befe52a3eac52d983b0dfae9cb8d58dfa0ede0648e1`  
		Last Modified: Thu, 21 Jan 2021 03:54:37 GMT  
		Size: 30.4 MB (30422854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a41aaf71d5cf82fa1f9e11d2d352906ae135d0b216c665ed76ad9a8e1ce046`  
		Last Modified: Thu, 21 Jan 2021 03:54:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e417a2309160c84b59c2e2ca585c0c1bd11a20876b7b04f00ed626592cc50e3`  
		Last Modified: Thu, 21 Jan 2021 06:29:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902524cdd9e3f0443a75babb289e129c0c2ec2b986161aa293ea8100cc77242b`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 5.6 MB (5630103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e198886a17e45226cfc6e3993ef55ca78556f6668984578c614bb01f0842e46`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 1.2 MB (1246925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953fb576afa139daf106d7a5511866370880e5a9b887ee386312bf0fcdd74d0`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d19ff23593668af110ba0e7d4a012fed889478daa306ab627946ff849286d5`  
		Last Modified: Thu, 21 Jan 2021 06:29:24 GMT  
		Size: 934.8 KB (934827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08451c7ddd7e19ffd1ed4c579ab92382506bedd27f02d3a0a9a481ef37b30887`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7b841158ff59be5418005816766fb3a79d97b14481688aad52d195b00fb654`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0e773762e9e799e50a66a4f5c9757ab1b9c3e22642ce1a349d9e0bccf1ebcd`  
		Last Modified: Thu, 21 Jan 2021 06:30:17 GMT  
		Size: 79.9 MB (79924102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8607404c5be8478cbb432cdcae5b24aaaebf1f59c54fcae6ffa9d685b0901c28`  
		Last Modified: Mon, 22 Feb 2021 23:50:20 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57907cace02e5b37ca3cb19bbd04bc9653b7980fbd1a53faa2f4ef9416a0302f`  
		Last Modified: Mon, 22 Feb 2021 23:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:c5def6a323de2180f4b30433c0a5b1f345577eb0ced884d03987a3758bad22fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:1dea8c253b82c3d433054d350b5ef2e357268583c6ca22d86994e75158539461
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107989412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1306fb20556f09a325088bb5de55cf7cb2313664aafc9e87146cff5b9848ccfb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 12:00:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 12:00:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:23 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 12:00:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 12:00:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 12:00:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 12:00:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 12:00:43 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:24:19 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:24:20 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:25:00 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:25:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:25:01 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:25:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:25:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:25:02 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:25:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e1d55d7187e8f362e53e468bc013ece20d08729dfa19233d4b201ea6c0fdd`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbd8eb6c494fbc05415014eca7a11f912cb7a6db85b18e0251e25aedb0f1cf`  
		Last Modified: Thu, 21 Jan 2021 12:04:31 GMT  
		Size: 4.8 MB (4811143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba484d25fdf813b30ca6199138092b8ed6ffa98bb5e742ad0d79e7057203632c`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.3 MB (1326584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3721839f3a0dcdcf6255072f1782da13e42a4068eb1eba2ec8fa8fd589289be`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0624c9c3aad26b62edc6088904a5782131a5b527711d3a6ac7ad4d663e492b83`  
		Last Modified: Thu, 21 Jan 2021 12:04:28 GMT  
		Size: 932.3 KB (932287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0756263074505a61315650e925f2530ee01ad1ea54bbd5cee32a20dc5b540973`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750a707bc293889adada0e840fc1981b1288f878d087f431dcb3a493783ed83`  
		Last Modified: Mon, 22 Feb 2021 23:26:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76da6d3fca8d3af98347bbe6e3a1f2fed6e9be5235c90027badbd41679da77f7`  
		Last Modified: Mon, 22 Feb 2021 23:27:12 GMT  
		Size: 74.2 MB (74196030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa65a7e9190db56435a9e4e5c017ac65cf4c5d8cd7a5268f199f4ac19c14d55`  
		Last Modified: Mon, 22 Feb 2021 23:26:57 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c755f0f8d7f2582d345bed2d502b6af84b43dfd6da0ecb862e5ae137bd040be6`  
		Last Modified: Mon, 22 Feb 2021 23:26:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fb8e50148b05b646106f4b058bd7c32a4b9fd03c49b383fc5308d3eae61502f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103142216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:297a6e549eaeaa81745409e77b02a72c6989675bc8b0729021b7d1bbac22de7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:43:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:43:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:43:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:44:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:44:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:44:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:44:21 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:44:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:44:24 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:00:18 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:00:21 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:01:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:01:15 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:01:16 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:01:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:01:20 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:01:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0913f7e8916a73df7595a8eed8504a0fe2b9a1ef0eb726442f2d3ddd62e6c29f`  
		Last Modified: Thu, 21 Jan 2021 05:49:13 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e8c54ecac617f1826858c0e6ca4c741eaa268f514e5bc12a9b9ff403c8c97c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 4.4 MB (4394730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de0e92bd62367167d5ecb0e93306cb8f77e9eda05a006fab36ad7843c3e06f`  
		Last Modified: Thu, 21 Jan 2021 05:49:10 GMT  
		Size: 1.3 MB (1263716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0265c953d9ee94de17c5d84e00c0dea2c5b71a1d022ecce588eae2d642ad5c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d8e12d2b1bb184b49dce9c2717a0adb1dca18e8c5f65ae57867ae5e8987b7`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 925.3 KB (925349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4a1e7930ee33a2c49dea2d0899a87a3f76ad932ba63f9ad479372bd8bab97`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337f6f1a89e8325930913b0980bab818f85c100b5085cca042278ff9384794a9`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7513c1433c3c2d4eaae0191906578dcb3435d8116aa922dd22505780e80a410`  
		Last Modified: Mon, 22 Feb 2021 23:04:21 GMT  
		Size: 72.8 MB (72812063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc9ca5af48c9f00f02c647fa85350fb5e786280938d2ed16080c4c935928c08`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b688387ec781d3aa1a2314b08d0cc8c750b1ef42ac217ac021208161727deb56`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:25cf2d0b35d0c9bf2a5ec0bd64539b3470ff2f3542fca00dd59a4711d7806fa5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116018459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b9a069377bbc70776a1e0c1762ae62aa20afc3151238a58736c715507c3417c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:03 GMT
ADD file:f6214eb5991df55aa5198d84442d6ddd28b67d4043d1832afba8b30e0249dcf5 in / 
# Thu, 21 Jan 2021 03:49:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:08:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 06:10:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:10:45 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 06:11:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 06:12:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 06:12:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:12:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 06:12:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:13:05 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:39:51 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:40:02 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:45:23 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:45:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:45:34 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:45:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:45:56 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:46:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e07786faec2ce77c08f20befe52a3eac52d983b0dfae9cb8d58dfa0ede0648e1`  
		Last Modified: Thu, 21 Jan 2021 03:54:37 GMT  
		Size: 30.4 MB (30422854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a41aaf71d5cf82fa1f9e11d2d352906ae135d0b216c665ed76ad9a8e1ce046`  
		Last Modified: Thu, 21 Jan 2021 03:54:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e417a2309160c84b59c2e2ca585c0c1bd11a20876b7b04f00ed626592cc50e3`  
		Last Modified: Thu, 21 Jan 2021 06:29:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902524cdd9e3f0443a75babb289e129c0c2ec2b986161aa293ea8100cc77242b`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 5.6 MB (5630103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e198886a17e45226cfc6e3993ef55ca78556f6668984578c614bb01f0842e46`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 1.2 MB (1246925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953fb576afa139daf106d7a5511866370880e5a9b887ee386312bf0fcdd74d0`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d19ff23593668af110ba0e7d4a012fed889478daa306ab627946ff849286d5`  
		Last Modified: Thu, 21 Jan 2021 06:29:24 GMT  
		Size: 934.8 KB (934827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08451c7ddd7e19ffd1ed4c579ab92382506bedd27f02d3a0a9a481ef37b30887`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98a472129753adbddf69c2cc4b21037f204134dd34f7e2265369d3e861b63b4`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fa159aff28d5d3871cd85fcda02edbbeff985b1303ef6a8689e0aa1abb0bb3`  
		Last Modified: Mon, 22 Feb 2021 23:50:01 GMT  
		Size: 77.8 MB (77770017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8067b821cfe80fa671ecf4faff700bb24be531a691ba5f538dd3b8de01ff4f85`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5982dd0ae12e6ae51378a9a0ce6924bab1b172528444fcd146b8f6260b75e7c`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.37`

```console
$ docker pull mariadb@sha256:c5def6a323de2180f4b30433c0a5b1f345577eb0ced884d03987a3758bad22fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.37` - linux; amd64

```console
$ docker pull mariadb@sha256:1dea8c253b82c3d433054d350b5ef2e357268583c6ca22d86994e75158539461
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107989412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1306fb20556f09a325088bb5de55cf7cb2313664aafc9e87146cff5b9848ccfb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 12:00:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 12:00:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:23 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 12:00:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 12:00:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 12:00:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 12:00:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 12:00:43 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:24:19 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:24:20 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:25:00 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:25:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:25:01 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:25:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:25:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:25:02 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:25:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e1d55d7187e8f362e53e468bc013ece20d08729dfa19233d4b201ea6c0fdd`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbd8eb6c494fbc05415014eca7a11f912cb7a6db85b18e0251e25aedb0f1cf`  
		Last Modified: Thu, 21 Jan 2021 12:04:31 GMT  
		Size: 4.8 MB (4811143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba484d25fdf813b30ca6199138092b8ed6ffa98bb5e742ad0d79e7057203632c`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.3 MB (1326584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3721839f3a0dcdcf6255072f1782da13e42a4068eb1eba2ec8fa8fd589289be`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0624c9c3aad26b62edc6088904a5782131a5b527711d3a6ac7ad4d663e492b83`  
		Last Modified: Thu, 21 Jan 2021 12:04:28 GMT  
		Size: 932.3 KB (932287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0756263074505a61315650e925f2530ee01ad1ea54bbd5cee32a20dc5b540973`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750a707bc293889adada0e840fc1981b1288f878d087f431dcb3a493783ed83`  
		Last Modified: Mon, 22 Feb 2021 23:26:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76da6d3fca8d3af98347bbe6e3a1f2fed6e9be5235c90027badbd41679da77f7`  
		Last Modified: Mon, 22 Feb 2021 23:27:12 GMT  
		Size: 74.2 MB (74196030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa65a7e9190db56435a9e4e5c017ac65cf4c5d8cd7a5268f199f4ac19c14d55`  
		Last Modified: Mon, 22 Feb 2021 23:26:57 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c755f0f8d7f2582d345bed2d502b6af84b43dfd6da0ecb862e5ae137bd040be6`  
		Last Modified: Mon, 22 Feb 2021 23:26:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fb8e50148b05b646106f4b058bd7c32a4b9fd03c49b383fc5308d3eae61502f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103142216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:297a6e549eaeaa81745409e77b02a72c6989675bc8b0729021b7d1bbac22de7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:43:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:43:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:43:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:44:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:44:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:44:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:44:21 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:44:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:44:24 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:00:18 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:00:21 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:01:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:01:15 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:01:16 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:01:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:01:20 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:01:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0913f7e8916a73df7595a8eed8504a0fe2b9a1ef0eb726442f2d3ddd62e6c29f`  
		Last Modified: Thu, 21 Jan 2021 05:49:13 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e8c54ecac617f1826858c0e6ca4c741eaa268f514e5bc12a9b9ff403c8c97c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 4.4 MB (4394730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de0e92bd62367167d5ecb0e93306cb8f77e9eda05a006fab36ad7843c3e06f`  
		Last Modified: Thu, 21 Jan 2021 05:49:10 GMT  
		Size: 1.3 MB (1263716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0265c953d9ee94de17c5d84e00c0dea2c5b71a1d022ecce588eae2d642ad5c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d8e12d2b1bb184b49dce9c2717a0adb1dca18e8c5f65ae57867ae5e8987b7`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 925.3 KB (925349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4a1e7930ee33a2c49dea2d0899a87a3f76ad932ba63f9ad479372bd8bab97`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337f6f1a89e8325930913b0980bab818f85c100b5085cca042278ff9384794a9`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7513c1433c3c2d4eaae0191906578dcb3435d8116aa922dd22505780e80a410`  
		Last Modified: Mon, 22 Feb 2021 23:04:21 GMT  
		Size: 72.8 MB (72812063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc9ca5af48c9f00f02c647fa85350fb5e786280938d2ed16080c4c935928c08`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b688387ec781d3aa1a2314b08d0cc8c750b1ef42ac217ac021208161727deb56`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37` - linux; ppc64le

```console
$ docker pull mariadb@sha256:25cf2d0b35d0c9bf2a5ec0bd64539b3470ff2f3542fca00dd59a4711d7806fa5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116018459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b9a069377bbc70776a1e0c1762ae62aa20afc3151238a58736c715507c3417c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:03 GMT
ADD file:f6214eb5991df55aa5198d84442d6ddd28b67d4043d1832afba8b30e0249dcf5 in / 
# Thu, 21 Jan 2021 03:49:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:08:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 06:10:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:10:45 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 06:11:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 06:12:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 06:12:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:12:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 06:12:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:13:05 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:39:51 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:40:02 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:45:23 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:45:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:45:34 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:45:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:45:56 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:46:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e07786faec2ce77c08f20befe52a3eac52d983b0dfae9cb8d58dfa0ede0648e1`  
		Last Modified: Thu, 21 Jan 2021 03:54:37 GMT  
		Size: 30.4 MB (30422854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a41aaf71d5cf82fa1f9e11d2d352906ae135d0b216c665ed76ad9a8e1ce046`  
		Last Modified: Thu, 21 Jan 2021 03:54:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e417a2309160c84b59c2e2ca585c0c1bd11a20876b7b04f00ed626592cc50e3`  
		Last Modified: Thu, 21 Jan 2021 06:29:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902524cdd9e3f0443a75babb289e129c0c2ec2b986161aa293ea8100cc77242b`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 5.6 MB (5630103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e198886a17e45226cfc6e3993ef55ca78556f6668984578c614bb01f0842e46`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 1.2 MB (1246925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953fb576afa139daf106d7a5511866370880e5a9b887ee386312bf0fcdd74d0`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d19ff23593668af110ba0e7d4a012fed889478daa306ab627946ff849286d5`  
		Last Modified: Thu, 21 Jan 2021 06:29:24 GMT  
		Size: 934.8 KB (934827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08451c7ddd7e19ffd1ed4c579ab92382506bedd27f02d3a0a9a481ef37b30887`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98a472129753adbddf69c2cc4b21037f204134dd34f7e2265369d3e861b63b4`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fa159aff28d5d3871cd85fcda02edbbeff985b1303ef6a8689e0aa1abb0bb3`  
		Last Modified: Mon, 22 Feb 2021 23:50:01 GMT  
		Size: 77.8 MB (77770017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8067b821cfe80fa671ecf4faff700bb24be531a691ba5f538dd3b8de01ff4f85`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5982dd0ae12e6ae51378a9a0ce6924bab1b172528444fcd146b8f6260b75e7c`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.37-bionic`

```console
$ docker pull mariadb@sha256:c5def6a323de2180f4b30433c0a5b1f345577eb0ced884d03987a3758bad22fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.37-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:1dea8c253b82c3d433054d350b5ef2e357268583c6ca22d86994e75158539461
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107989412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1306fb20556f09a325088bb5de55cf7cb2313664aafc9e87146cff5b9848ccfb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 12:00:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 12:00:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:23 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 12:00:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 12:00:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 12:00:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 12:00:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 12:00:43 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:24:19 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:24:20 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:25:00 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:25:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:25:01 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:25:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:25:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:25:02 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:25:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e1d55d7187e8f362e53e468bc013ece20d08729dfa19233d4b201ea6c0fdd`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbd8eb6c494fbc05415014eca7a11f912cb7a6db85b18e0251e25aedb0f1cf`  
		Last Modified: Thu, 21 Jan 2021 12:04:31 GMT  
		Size: 4.8 MB (4811143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba484d25fdf813b30ca6199138092b8ed6ffa98bb5e742ad0d79e7057203632c`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.3 MB (1326584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3721839f3a0dcdcf6255072f1782da13e42a4068eb1eba2ec8fa8fd589289be`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0624c9c3aad26b62edc6088904a5782131a5b527711d3a6ac7ad4d663e492b83`  
		Last Modified: Thu, 21 Jan 2021 12:04:28 GMT  
		Size: 932.3 KB (932287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0756263074505a61315650e925f2530ee01ad1ea54bbd5cee32a20dc5b540973`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750a707bc293889adada0e840fc1981b1288f878d087f431dcb3a493783ed83`  
		Last Modified: Mon, 22 Feb 2021 23:26:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76da6d3fca8d3af98347bbe6e3a1f2fed6e9be5235c90027badbd41679da77f7`  
		Last Modified: Mon, 22 Feb 2021 23:27:12 GMT  
		Size: 74.2 MB (74196030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa65a7e9190db56435a9e4e5c017ac65cf4c5d8cd7a5268f199f4ac19c14d55`  
		Last Modified: Mon, 22 Feb 2021 23:26:57 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c755f0f8d7f2582d345bed2d502b6af84b43dfd6da0ecb862e5ae137bd040be6`  
		Last Modified: Mon, 22 Feb 2021 23:26:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fb8e50148b05b646106f4b058bd7c32a4b9fd03c49b383fc5308d3eae61502f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103142216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:297a6e549eaeaa81745409e77b02a72c6989675bc8b0729021b7d1bbac22de7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:43:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:43:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:43:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:44:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:44:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:44:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:44:21 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:44:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:44:24 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:00:18 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:00:21 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:01:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:01:15 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:01:16 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:01:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:01:20 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:01:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0913f7e8916a73df7595a8eed8504a0fe2b9a1ef0eb726442f2d3ddd62e6c29f`  
		Last Modified: Thu, 21 Jan 2021 05:49:13 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e8c54ecac617f1826858c0e6ca4c741eaa268f514e5bc12a9b9ff403c8c97c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 4.4 MB (4394730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de0e92bd62367167d5ecb0e93306cb8f77e9eda05a006fab36ad7843c3e06f`  
		Last Modified: Thu, 21 Jan 2021 05:49:10 GMT  
		Size: 1.3 MB (1263716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0265c953d9ee94de17c5d84e00c0dea2c5b71a1d022ecce588eae2d642ad5c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d8e12d2b1bb184b49dce9c2717a0adb1dca18e8c5f65ae57867ae5e8987b7`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 925.3 KB (925349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4a1e7930ee33a2c49dea2d0899a87a3f76ad932ba63f9ad479372bd8bab97`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337f6f1a89e8325930913b0980bab818f85c100b5085cca042278ff9384794a9`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7513c1433c3c2d4eaae0191906578dcb3435d8116aa922dd22505780e80a410`  
		Last Modified: Mon, 22 Feb 2021 23:04:21 GMT  
		Size: 72.8 MB (72812063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc9ca5af48c9f00f02c647fa85350fb5e786280938d2ed16080c4c935928c08`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b688387ec781d3aa1a2314b08d0cc8c750b1ef42ac217ac021208161727deb56`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.37-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:25cf2d0b35d0c9bf2a5ec0bd64539b3470ff2f3542fca00dd59a4711d7806fa5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116018459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b9a069377bbc70776a1e0c1762ae62aa20afc3151238a58736c715507c3417c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:03 GMT
ADD file:f6214eb5991df55aa5198d84442d6ddd28b67d4043d1832afba8b30e0249dcf5 in / 
# Thu, 21 Jan 2021 03:49:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:08:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 06:10:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:10:45 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 06:11:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 06:12:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 06:12:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:12:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 06:12:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:13:05 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:39:51 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:40:02 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:45:23 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:45:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:45:34 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:45:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:45:56 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:46:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e07786faec2ce77c08f20befe52a3eac52d983b0dfae9cb8d58dfa0ede0648e1`  
		Last Modified: Thu, 21 Jan 2021 03:54:37 GMT  
		Size: 30.4 MB (30422854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a41aaf71d5cf82fa1f9e11d2d352906ae135d0b216c665ed76ad9a8e1ce046`  
		Last Modified: Thu, 21 Jan 2021 03:54:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e417a2309160c84b59c2e2ca585c0c1bd11a20876b7b04f00ed626592cc50e3`  
		Last Modified: Thu, 21 Jan 2021 06:29:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902524cdd9e3f0443a75babb289e129c0c2ec2b986161aa293ea8100cc77242b`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 5.6 MB (5630103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e198886a17e45226cfc6e3993ef55ca78556f6668984578c614bb01f0842e46`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 1.2 MB (1246925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953fb576afa139daf106d7a5511866370880e5a9b887ee386312bf0fcdd74d0`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d19ff23593668af110ba0e7d4a012fed889478daa306ab627946ff849286d5`  
		Last Modified: Thu, 21 Jan 2021 06:29:24 GMT  
		Size: 934.8 KB (934827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08451c7ddd7e19ffd1ed4c579ab92382506bedd27f02d3a0a9a481ef37b30887`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98a472129753adbddf69c2cc4b21037f204134dd34f7e2265369d3e861b63b4`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fa159aff28d5d3871cd85fcda02edbbeff985b1303ef6a8689e0aa1abb0bb3`  
		Last Modified: Mon, 22 Feb 2021 23:50:01 GMT  
		Size: 77.8 MB (77770017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8067b821cfe80fa671ecf4faff700bb24be531a691ba5f538dd3b8de01ff4f85`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5982dd0ae12e6ae51378a9a0ce6924bab1b172528444fcd146b8f6260b75e7c`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:c5def6a323de2180f4b30433c0a5b1f345577eb0ced884d03987a3758bad22fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:1dea8c253b82c3d433054d350b5ef2e357268583c6ca22d86994e75158539461
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107989412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1306fb20556f09a325088bb5de55cf7cb2313664aafc9e87146cff5b9848ccfb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:37:59 GMT
ADD file:ef36fee25b0bd1d99979ecb8d54b206cec33d4e8fd2232189f0d8e5ab9754798 in / 
# Thu, 21 Jan 2021 03:38:01 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:05 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 12:00:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 12:00:23 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:23 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 12:00:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 12:00:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 12:00:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 12:00:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 12:00:42 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 12:00:43 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:24:19 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:24:20 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:25:00 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:25:00 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:25:01 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:25:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:25:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:25:02 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:25:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d519e2592276828ca171d85e0532899cd4f98c70f5c697b45fa2e126e9f9fe49`  
		Last Modified: Thu, 21 Jan 2021 03:40:27 GMT  
		Size: 26.7 MB (26709716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d2dfcfa9cd230ed3c47defec2670d45081598c721dd85cafc34ea459f970e`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3afe92c540b778c64ca316d1e679d55d2d2e812e450f516a808ee591f0c3f77`  
		Last Modified: Thu, 21 Jan 2021 03:40:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e1d55d7187e8f362e53e468bc013ece20d08729dfa19233d4b201ea6c0fdd`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bbd8eb6c494fbc05415014eca7a11f912cb7a6db85b18e0251e25aedb0f1cf`  
		Last Modified: Thu, 21 Jan 2021 12:04:31 GMT  
		Size: 4.8 MB (4811143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba484d25fdf813b30ca6199138092b8ed6ffa98bb5e742ad0d79e7057203632c`  
		Last Modified: Thu, 21 Jan 2021 12:04:29 GMT  
		Size: 1.3 MB (1326584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3721839f3a0dcdcf6255072f1782da13e42a4068eb1eba2ec8fa8fd589289be`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0624c9c3aad26b62edc6088904a5782131a5b527711d3a6ac7ad4d663e492b83`  
		Last Modified: Thu, 21 Jan 2021 12:04:28 GMT  
		Size: 932.3 KB (932287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0756263074505a61315650e925f2530ee01ad1ea54bbd5cee32a20dc5b540973`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 5.2 KB (5171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750a707bc293889adada0e840fc1981b1288f878d087f431dcb3a493783ed83`  
		Last Modified: Mon, 22 Feb 2021 23:26:57 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76da6d3fca8d3af98347bbe6e3a1f2fed6e9be5235c90027badbd41679da77f7`  
		Last Modified: Mon, 22 Feb 2021 23:27:12 GMT  
		Size: 74.2 MB (74196030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa65a7e9190db56435a9e4e5c017ac65cf4c5d8cd7a5268f199f4ac19c14d55`  
		Last Modified: Mon, 22 Feb 2021 23:26:57 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c755f0f8d7f2582d345bed2d502b6af84b43dfd6da0ecb862e5ae137bd040be6`  
		Last Modified: Mon, 22 Feb 2021 23:26:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:fb8e50148b05b646106f4b058bd7c32a4b9fd03c49b383fc5308d3eae61502f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103142216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:297a6e549eaeaa81745409e77b02a72c6989675bc8b0729021b7d1bbac22de7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:23 GMT
ADD file:7d9bc01cf1f3757bf5fa308213a77aeb128883cc13616ff46b3da5b0e65b92f2 in / 
# Thu, 21 Jan 2021 03:49:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:29 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:49:32 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:43:30 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:43:47 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:43:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:44:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:44:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:44:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:44:21 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:44:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:44:24 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:00:18 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:00:21 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:01:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:01:15 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:01:16 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:01:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:01:20 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:01:21 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:64e3fba066352e44a4c1eeb6caedc87c29b46f0a7b31e21a58183fc8370005bd`  
		Last Modified: Tue, 19 Jan 2021 00:25:17 GMT  
		Size: 23.7 MB (23732640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb433f451339aab734bb52e3df5b34cdea477f3f8e3aa32f7ac060bd852de2`  
		Last Modified: Thu, 21 Jan 2021 03:51:55 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3042a0d94b83caeb29bc20734c197130f58e14e86e8e6cdad8b768052bb563c`  
		Last Modified: Thu, 21 Jan 2021 03:51:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0913f7e8916a73df7595a8eed8504a0fe2b9a1ef0eb726442f2d3ddd62e6c29f`  
		Last Modified: Thu, 21 Jan 2021 05:49:13 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e8c54ecac617f1826858c0e6ca4c741eaa268f514e5bc12a9b9ff403c8c97c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 4.4 MB (4394730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de0e92bd62367167d5ecb0e93306cb8f77e9eda05a006fab36ad7843c3e06f`  
		Last Modified: Thu, 21 Jan 2021 05:49:10 GMT  
		Size: 1.3 MB (1263716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0265c953d9ee94de17c5d84e00c0dea2c5b71a1d022ecce588eae2d642ad5c`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33d8e12d2b1bb184b49dce9c2717a0adb1dca18e8c5f65ae57867ae5e8987b7`  
		Last Modified: Thu, 21 Jan 2021 05:49:12 GMT  
		Size: 925.3 KB (925349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4a1e7930ee33a2c49dea2d0899a87a3f76ad932ba63f9ad479372bd8bab97`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 5.2 KB (5172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337f6f1a89e8325930913b0980bab818f85c100b5085cca042278ff9384794a9`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7513c1433c3c2d4eaae0191906578dcb3435d8116aa922dd22505780e80a410`  
		Last Modified: Mon, 22 Feb 2021 23:04:21 GMT  
		Size: 72.8 MB (72812063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc9ca5af48c9f00f02c647fa85350fb5e786280938d2ed16080c4c935928c08`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b688387ec781d3aa1a2314b08d0cc8c750b1ef42ac217ac021208161727deb56`  
		Last Modified: Mon, 22 Feb 2021 23:03:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:25cf2d0b35d0c9bf2a5ec0bd64539b3470ff2f3542fca00dd59a4711d7806fa5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116018459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b9a069377bbc70776a1e0c1762ae62aa20afc3151238a58736c715507c3417c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:03 GMT
ADD file:f6214eb5991df55aa5198d84442d6ddd28b67d4043d1832afba8b30e0249dcf5 in / 
# Thu, 21 Jan 2021 03:49:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:09 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 06:08:55 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 06:10:37 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:10:45 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 06:11:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 06:12:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 06:12:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 06:12:36 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 06:12:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:13:05 GMT
ENV MARIADB_MAJOR=10.2
# Mon, 22 Feb 2021 23:39:51 GMT
ENV MARIADB_VERSION=1:10.2.37+maria~bionic
# Mon, 22 Feb 2021 23:40:02 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:45:23 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:45:31 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:45:34 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:45:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:45:56 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:46:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e07786faec2ce77c08f20befe52a3eac52d983b0dfae9cb8d58dfa0ede0648e1`  
		Last Modified: Thu, 21 Jan 2021 03:54:37 GMT  
		Size: 30.4 MB (30422854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a41aaf71d5cf82fa1f9e11d2d352906ae135d0b216c665ed76ad9a8e1ce046`  
		Last Modified: Thu, 21 Jan 2021 03:54:30 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e417a2309160c84b59c2e2ca585c0c1bd11a20876b7b04f00ed626592cc50e3`  
		Last Modified: Thu, 21 Jan 2021 06:29:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902524cdd9e3f0443a75babb289e129c0c2ec2b986161aa293ea8100cc77242b`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 5.6 MB (5630103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e198886a17e45226cfc6e3993ef55ca78556f6668984578c614bb01f0842e46`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 1.2 MB (1246925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953fb576afa139daf106d7a5511866370880e5a9b887ee386312bf0fcdd74d0`  
		Last Modified: Thu, 21 Jan 2021 06:29:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d19ff23593668af110ba0e7d4a012fed889478daa306ab627946ff849286d5`  
		Last Modified: Thu, 21 Jan 2021 06:29:24 GMT  
		Size: 934.8 KB (934827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08451c7ddd7e19ffd1ed4c579ab92382506bedd27f02d3a0a9a481ef37b30887`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 5.2 KB (5174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98a472129753adbddf69c2cc4b21037f204134dd34f7e2265369d3e861b63b4`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fa159aff28d5d3871cd85fcda02edbbeff985b1303ef6a8689e0aa1abb0bb3`  
		Last Modified: Mon, 22 Feb 2021 23:50:01 GMT  
		Size: 77.8 MB (77770017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8067b821cfe80fa671ecf4faff700bb24be531a691ba5f538dd3b8de01ff4f85`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5982dd0ae12e6ae51378a9a0ce6924bab1b172528444fcd146b8f6260b75e7c`  
		Last Modified: Mon, 22 Feb 2021 23:49:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:3bcf2b43240e37aacce0beee541b6e07afd7b0fe0ea3a2d8ae6dbce6e74f1c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:ec729effa8745d23e1e37d48bafa7e5ca9d1105a441e285cd76464c4ad1b393b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118342352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a27c6050400f9c119883482ce5d43d9125c6be7929c01ec3d48a6d91c8f97eca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:59:23 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 23:23:38 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 23:23:39 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:24:08 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:24:08 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:24:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:24:09 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:24:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8087b9eabae289ac012c3e301cf27aad67eee75110db7d2cc9a540d0328aafcf`  
		Last Modified: Mon, 22 Feb 2021 23:26:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c31a50c54658b3907af3cce9bc0879d9039fc569218d2fefa0343cadaa67cd`  
		Last Modified: Mon, 22 Feb 2021 23:26:50 GMT  
		Size: 81.7 MB (81680790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6246ce3ce1c1245653e30a327ba20a1a7db5fbf4b90b90fba0c694ea3d183ca4`  
		Last Modified: Mon, 22 Feb 2021 23:26:34 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b23c53e986c3738a86ae9eafdd6cf846e83a02211311217f47d785df466cd`  
		Last Modified: Mon, 22 Feb 2021 23:26:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:aa35ff5af0db26c07190132f632622c6568fc89aaa034e9d9bd8a700ba9b2017
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116034743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a186f3e1b690f3ec18cdf733791b8fbed10cea8f5a2625b5dac98938b9a4ab0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:42:21 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 22:58:58 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 22:59:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:59:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:59:59 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:00:00 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:00:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:00:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:00:05 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:00:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6f2710954a4eda3a066655b49c18f7eb39c62e5088fdf33301e0d2ddbefcb4`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8109e16b1ea03ef5efb1d4564a841cdc864340c8fa817d76e2ef37bf952dc79`  
		Last Modified: Mon, 22 Feb 2021 23:03:47 GMT  
		Size: 80.9 MB (80861647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd1aea6c00abe6be1d2b7a17eccb8e99d31c5c3730f854b5cc13740302b81be`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7079158e5939f34d1e6477609720ee6aa1211748585bf291dc57d362d0ab1be4`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:91b31734e1243e34fa6bf1fefd4589775a60a30f26d1b53c9334c63b0eaa9dc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128922072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4713c1142ff1cb0e30943a8ff17cabc66f776891680dc7f9012bd6e338dca77c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:03:47 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 23:34:10 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 23:34:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:38:51 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:38:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:38:57 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:39:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:39:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:39:20 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:39:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c09c0e2d484dd0f0ba166d0807490d53501b022ce3a9549932457b1e18de511`  
		Last Modified: Mon, 22 Feb 2021 23:49:08 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5395fc0f1bd30eeebbfbdc93bf0da122c7e6e20d283b1cfbda9653b031d5d29d`  
		Last Modified: Mon, 22 Feb 2021 23:49:27 GMT  
		Size: 86.4 MB (86437033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44ee7c21db9932d8fa444d03c1766fe9dbbd053ed7455aed2ed2c2c9c9fe5e2`  
		Last Modified: Mon, 22 Feb 2021 23:49:09 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5136bec1e3fe48b812a14ebb027b75e7ec3558ac9b1dd8c792a9d0261b5f3c`  
		Last Modified: Mon, 22 Feb 2021 23:49:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.28`

```console
$ docker pull mariadb@sha256:3bcf2b43240e37aacce0beee541b6e07afd7b0fe0ea3a2d8ae6dbce6e74f1c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.28` - linux; amd64

```console
$ docker pull mariadb@sha256:ec729effa8745d23e1e37d48bafa7e5ca9d1105a441e285cd76464c4ad1b393b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118342352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a27c6050400f9c119883482ce5d43d9125c6be7929c01ec3d48a6d91c8f97eca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:59:23 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 23:23:38 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 23:23:39 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:24:08 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:24:08 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:24:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:24:09 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:24:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8087b9eabae289ac012c3e301cf27aad67eee75110db7d2cc9a540d0328aafcf`  
		Last Modified: Mon, 22 Feb 2021 23:26:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c31a50c54658b3907af3cce9bc0879d9039fc569218d2fefa0343cadaa67cd`  
		Last Modified: Mon, 22 Feb 2021 23:26:50 GMT  
		Size: 81.7 MB (81680790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6246ce3ce1c1245653e30a327ba20a1a7db5fbf4b90b90fba0c694ea3d183ca4`  
		Last Modified: Mon, 22 Feb 2021 23:26:34 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b23c53e986c3738a86ae9eafdd6cf846e83a02211311217f47d785df466cd`  
		Last Modified: Mon, 22 Feb 2021 23:26:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:aa35ff5af0db26c07190132f632622c6568fc89aaa034e9d9bd8a700ba9b2017
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116034743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a186f3e1b690f3ec18cdf733791b8fbed10cea8f5a2625b5dac98938b9a4ab0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:42:21 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 22:58:58 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 22:59:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:59:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:59:59 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:00:00 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:00:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:00:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:00:05 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:00:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6f2710954a4eda3a066655b49c18f7eb39c62e5088fdf33301e0d2ddbefcb4`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8109e16b1ea03ef5efb1d4564a841cdc864340c8fa817d76e2ef37bf952dc79`  
		Last Modified: Mon, 22 Feb 2021 23:03:47 GMT  
		Size: 80.9 MB (80861647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd1aea6c00abe6be1d2b7a17eccb8e99d31c5c3730f854b5cc13740302b81be`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7079158e5939f34d1e6477609720ee6aa1211748585bf291dc57d362d0ab1be4`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28` - linux; ppc64le

```console
$ docker pull mariadb@sha256:91b31734e1243e34fa6bf1fefd4589775a60a30f26d1b53c9334c63b0eaa9dc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128922072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4713c1142ff1cb0e30943a8ff17cabc66f776891680dc7f9012bd6e338dca77c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:03:47 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 23:34:10 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 23:34:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:38:51 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:38:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:38:57 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:39:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:39:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:39:20 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:39:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c09c0e2d484dd0f0ba166d0807490d53501b022ce3a9549932457b1e18de511`  
		Last Modified: Mon, 22 Feb 2021 23:49:08 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5395fc0f1bd30eeebbfbdc93bf0da122c7e6e20d283b1cfbda9653b031d5d29d`  
		Last Modified: Mon, 22 Feb 2021 23:49:27 GMT  
		Size: 86.4 MB (86437033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44ee7c21db9932d8fa444d03c1766fe9dbbd053ed7455aed2ed2c2c9c9fe5e2`  
		Last Modified: Mon, 22 Feb 2021 23:49:09 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5136bec1e3fe48b812a14ebb027b75e7ec3558ac9b1dd8c792a9d0261b5f3c`  
		Last Modified: Mon, 22 Feb 2021 23:49:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.28-focal`

```console
$ docker pull mariadb@sha256:3bcf2b43240e37aacce0beee541b6e07afd7b0fe0ea3a2d8ae6dbce6e74f1c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.28-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:ec729effa8745d23e1e37d48bafa7e5ca9d1105a441e285cd76464c4ad1b393b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118342352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a27c6050400f9c119883482ce5d43d9125c6be7929c01ec3d48a6d91c8f97eca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:59:23 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 23:23:38 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 23:23:39 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:24:08 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:24:08 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:24:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:24:09 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:24:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8087b9eabae289ac012c3e301cf27aad67eee75110db7d2cc9a540d0328aafcf`  
		Last Modified: Mon, 22 Feb 2021 23:26:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c31a50c54658b3907af3cce9bc0879d9039fc569218d2fefa0343cadaa67cd`  
		Last Modified: Mon, 22 Feb 2021 23:26:50 GMT  
		Size: 81.7 MB (81680790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6246ce3ce1c1245653e30a327ba20a1a7db5fbf4b90b90fba0c694ea3d183ca4`  
		Last Modified: Mon, 22 Feb 2021 23:26:34 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b23c53e986c3738a86ae9eafdd6cf846e83a02211311217f47d785df466cd`  
		Last Modified: Mon, 22 Feb 2021 23:26:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:aa35ff5af0db26c07190132f632622c6568fc89aaa034e9d9bd8a700ba9b2017
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116034743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a186f3e1b690f3ec18cdf733791b8fbed10cea8f5a2625b5dac98938b9a4ab0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:42:21 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 22:58:58 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 22:59:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:59:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:59:59 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:00:00 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:00:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:00:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:00:05 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:00:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6f2710954a4eda3a066655b49c18f7eb39c62e5088fdf33301e0d2ddbefcb4`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8109e16b1ea03ef5efb1d4564a841cdc864340c8fa817d76e2ef37bf952dc79`  
		Last Modified: Mon, 22 Feb 2021 23:03:47 GMT  
		Size: 80.9 MB (80861647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd1aea6c00abe6be1d2b7a17eccb8e99d31c5c3730f854b5cc13740302b81be`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7079158e5939f34d1e6477609720ee6aa1211748585bf291dc57d362d0ab1be4`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.28-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:91b31734e1243e34fa6bf1fefd4589775a60a30f26d1b53c9334c63b0eaa9dc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128922072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4713c1142ff1cb0e30943a8ff17cabc66f776891680dc7f9012bd6e338dca77c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:03:47 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 23:34:10 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 23:34:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:38:51 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:38:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:38:57 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:39:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:39:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:39:20 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:39:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c09c0e2d484dd0f0ba166d0807490d53501b022ce3a9549932457b1e18de511`  
		Last Modified: Mon, 22 Feb 2021 23:49:08 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5395fc0f1bd30eeebbfbdc93bf0da122c7e6e20d283b1cfbda9653b031d5d29d`  
		Last Modified: Mon, 22 Feb 2021 23:49:27 GMT  
		Size: 86.4 MB (86437033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44ee7c21db9932d8fa444d03c1766fe9dbbd053ed7455aed2ed2c2c9c9fe5e2`  
		Last Modified: Mon, 22 Feb 2021 23:49:09 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5136bec1e3fe48b812a14ebb027b75e7ec3558ac9b1dd8c792a9d0261b5f3c`  
		Last Modified: Mon, 22 Feb 2021 23:49:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:3bcf2b43240e37aacce0beee541b6e07afd7b0fe0ea3a2d8ae6dbce6e74f1c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:ec729effa8745d23e1e37d48bafa7e5ca9d1105a441e285cd76464c4ad1b393b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118342352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a27c6050400f9c119883482ce5d43d9125c6be7929c01ec3d48a6d91c8f97eca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:59:23 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 23:23:38 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 23:23:39 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:24:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:24:08 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:24:08 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:24:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:24:09 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:24:10 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8087b9eabae289ac012c3e301cf27aad67eee75110db7d2cc9a540d0328aafcf`  
		Last Modified: Mon, 22 Feb 2021 23:26:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c31a50c54658b3907af3cce9bc0879d9039fc569218d2fefa0343cadaa67cd`  
		Last Modified: Mon, 22 Feb 2021 23:26:50 GMT  
		Size: 81.7 MB (81680790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6246ce3ce1c1245653e30a327ba20a1a7db5fbf4b90b90fba0c694ea3d183ca4`  
		Last Modified: Mon, 22 Feb 2021 23:26:34 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b23c53e986c3738a86ae9eafdd6cf846e83a02211311217f47d785df466cd`  
		Last Modified: Mon, 22 Feb 2021 23:26:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:aa35ff5af0db26c07190132f632622c6568fc89aaa034e9d9bd8a700ba9b2017
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (116034743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a186f3e1b690f3ec18cdf733791b8fbed10cea8f5a2625b5dac98938b9a4ab0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:42:21 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 22:58:58 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 22:59:00 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:59:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:59:59 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:00:00 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:00:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:00:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:00:05 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:00:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6f2710954a4eda3a066655b49c18f7eb39c62e5088fdf33301e0d2ddbefcb4`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8109e16b1ea03ef5efb1d4564a841cdc864340c8fa817d76e2ef37bf952dc79`  
		Last Modified: Mon, 22 Feb 2021 23:03:47 GMT  
		Size: 80.9 MB (80861647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd1aea6c00abe6be1d2b7a17eccb8e99d31c5c3730f854b5cc13740302b81be`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 5.0 KB (5033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7079158e5939f34d1e6477609720ee6aa1211748585bf291dc57d362d0ab1be4`  
		Last Modified: Mon, 22 Feb 2021 23:03:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:91b31734e1243e34fa6bf1fefd4589775a60a30f26d1b53c9334c63b0eaa9dc8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128922072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4713c1142ff1cb0e30943a8ff17cabc66f776891680dc7f9012bd6e338dca77c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 06:03:47 GMT
ENV MARIADB_MAJOR=10.3
# Mon, 22 Feb 2021 23:34:10 GMT
ENV MARIADB_VERSION=1:10.3.28+maria~focal
# Mon, 22 Feb 2021 23:34:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:38:51 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:38:55 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:38:57 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:39:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:39:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:39:20 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:39:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c09c0e2d484dd0f0ba166d0807490d53501b022ce3a9549932457b1e18de511`  
		Last Modified: Mon, 22 Feb 2021 23:49:08 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5395fc0f1bd30eeebbfbdc93bf0da122c7e6e20d283b1cfbda9653b031d5d29d`  
		Last Modified: Mon, 22 Feb 2021 23:49:27 GMT  
		Size: 86.4 MB (86437033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44ee7c21db9932d8fa444d03c1766fe9dbbd053ed7455aed2ed2c2c9c9fe5e2`  
		Last Modified: Mon, 22 Feb 2021 23:49:09 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5136bec1e3fe48b812a14ebb027b75e7ec3558ac9b1dd8c792a9d0261b5f3c`  
		Last Modified: Mon, 22 Feb 2021 23:49:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:32270ca5ee62505b8bd83e067e2626d593bec0560bcd4a60e434217089d7ee6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:b519bfc7b05083f03022b11c7a37c2695da7ca3722494864ee38e2ca75dd823c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122219654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891015ba0a338897130cad7372ed9f00fcf77b7b7994b1d08bdaa5c53e831b84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:49 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 23:22:58 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 23:22:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:23:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:23:28 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:23:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:23:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:23:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:23:30 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:23:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb9a01d184e1cd0cd08617495ad1c00af608b11ed14a1aee9754a4e05368532`  
		Last Modified: Mon, 22 Feb 2021 23:26:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde85630a882d56d9e2de097ffc514022b495298f16bef8f8720ee551882ed2`  
		Last Modified: Mon, 22 Feb 2021 23:26:26 GMT  
		Size: 85.6 MB (85558093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24a97a3b501e62738d8a0e12578e43822ea4967d60298dd2506c0339bd52d0c`  
		Last Modified: Mon, 22 Feb 2021 23:26:08 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca65e5a3bb7246d40b27cb04d040b40cf2e04ca3212774f20649b2d54461ead`  
		Last Modified: Mon, 22 Feb 2021 23:26:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6a2a842442924080424f2f1ee93456ba2e164b6e82b60e2889873ca196fe02b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119803703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8500688c5aadb99309719909ca2270d850e0f5164880d402602fa462c93e7590`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:41:23 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 22:57:51 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 22:57:53 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:58:39 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:58:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:58:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 22:58:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:58:43 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:58:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f68101bda465d0def90d1bff9ad859863a6a7324bffd75603f1247b38b1b6b9`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56f366246440a01af255c8653a35ec73c718160d30d24532ddef7bf179d826`  
		Last Modified: Mon, 22 Feb 2021 23:03:14 GMT  
		Size: 84.6 MB (84630606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277679070e81c5f1c2e0f4f6867057b442bcf3c8f8934c366c957e39a56c9506`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24665aa55fbb701500b33fba88fa3535bcb91942d0ece77a3ba7891c597837a`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4afbf91d452ffd2ba54be842a1a4b7d43c5ccbec19f8ab06f04a588b3806371c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132601058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296be39e4a521d5333ea340c6f961db79b331ff95706ab04d4e6259cbd6cc0e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:59:02 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 23:27:31 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 23:27:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:32:43 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:32:51 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:32:55 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:33:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:33:32 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:33:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028e2c33df93b6273c68e3ee47798c813fc1dfec069d9f7026f42da2d00bab1`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704db790ada8d22d0f8b7cc92f07cbe3189530818d890574cdbeac376df7c104`  
		Last Modified: Mon, 22 Feb 2021 23:48:48 GMT  
		Size: 90.1 MB (90116019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3480e0e5f746ea13135811926708c0265082b91c0ae12683d1747190fb5847`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eaeed5ac21d3ea1002610bdc4f4811cec9a0eb173406edc042f505622b39ee`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.18`

```console
$ docker pull mariadb@sha256:32270ca5ee62505b8bd83e067e2626d593bec0560bcd4a60e434217089d7ee6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.18` - linux; amd64

```console
$ docker pull mariadb@sha256:b519bfc7b05083f03022b11c7a37c2695da7ca3722494864ee38e2ca75dd823c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122219654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891015ba0a338897130cad7372ed9f00fcf77b7b7994b1d08bdaa5c53e831b84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:49 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 23:22:58 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 23:22:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:23:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:23:28 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:23:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:23:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:23:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:23:30 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:23:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb9a01d184e1cd0cd08617495ad1c00af608b11ed14a1aee9754a4e05368532`  
		Last Modified: Mon, 22 Feb 2021 23:26:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde85630a882d56d9e2de097ffc514022b495298f16bef8f8720ee551882ed2`  
		Last Modified: Mon, 22 Feb 2021 23:26:26 GMT  
		Size: 85.6 MB (85558093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24a97a3b501e62738d8a0e12578e43822ea4967d60298dd2506c0339bd52d0c`  
		Last Modified: Mon, 22 Feb 2021 23:26:08 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca65e5a3bb7246d40b27cb04d040b40cf2e04ca3212774f20649b2d54461ead`  
		Last Modified: Mon, 22 Feb 2021 23:26:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6a2a842442924080424f2f1ee93456ba2e164b6e82b60e2889873ca196fe02b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119803703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8500688c5aadb99309719909ca2270d850e0f5164880d402602fa462c93e7590`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:41:23 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 22:57:51 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 22:57:53 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:58:39 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:58:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:58:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 22:58:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:58:43 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:58:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f68101bda465d0def90d1bff9ad859863a6a7324bffd75603f1247b38b1b6b9`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56f366246440a01af255c8653a35ec73c718160d30d24532ddef7bf179d826`  
		Last Modified: Mon, 22 Feb 2021 23:03:14 GMT  
		Size: 84.6 MB (84630606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277679070e81c5f1c2e0f4f6867057b442bcf3c8f8934c366c957e39a56c9506`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24665aa55fbb701500b33fba88fa3535bcb91942d0ece77a3ba7891c597837a`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4afbf91d452ffd2ba54be842a1a4b7d43c5ccbec19f8ab06f04a588b3806371c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132601058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296be39e4a521d5333ea340c6f961db79b331ff95706ab04d4e6259cbd6cc0e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:59:02 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 23:27:31 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 23:27:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:32:43 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:32:51 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:32:55 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:33:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:33:32 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:33:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028e2c33df93b6273c68e3ee47798c813fc1dfec069d9f7026f42da2d00bab1`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704db790ada8d22d0f8b7cc92f07cbe3189530818d890574cdbeac376df7c104`  
		Last Modified: Mon, 22 Feb 2021 23:48:48 GMT  
		Size: 90.1 MB (90116019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3480e0e5f746ea13135811926708c0265082b91c0ae12683d1747190fb5847`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eaeed5ac21d3ea1002610bdc4f4811cec9a0eb173406edc042f505622b39ee`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.18-focal`

```console
$ docker pull mariadb@sha256:32270ca5ee62505b8bd83e067e2626d593bec0560bcd4a60e434217089d7ee6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.18-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:b519bfc7b05083f03022b11c7a37c2695da7ca3722494864ee38e2ca75dd823c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122219654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891015ba0a338897130cad7372ed9f00fcf77b7b7994b1d08bdaa5c53e831b84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:49 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 23:22:58 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 23:22:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:23:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:23:28 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:23:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:23:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:23:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:23:30 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:23:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb9a01d184e1cd0cd08617495ad1c00af608b11ed14a1aee9754a4e05368532`  
		Last Modified: Mon, 22 Feb 2021 23:26:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde85630a882d56d9e2de097ffc514022b495298f16bef8f8720ee551882ed2`  
		Last Modified: Mon, 22 Feb 2021 23:26:26 GMT  
		Size: 85.6 MB (85558093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24a97a3b501e62738d8a0e12578e43822ea4967d60298dd2506c0339bd52d0c`  
		Last Modified: Mon, 22 Feb 2021 23:26:08 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca65e5a3bb7246d40b27cb04d040b40cf2e04ca3212774f20649b2d54461ead`  
		Last Modified: Mon, 22 Feb 2021 23:26:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6a2a842442924080424f2f1ee93456ba2e164b6e82b60e2889873ca196fe02b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119803703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8500688c5aadb99309719909ca2270d850e0f5164880d402602fa462c93e7590`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:41:23 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 22:57:51 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 22:57:53 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:58:39 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:58:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:58:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 22:58:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:58:43 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:58:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f68101bda465d0def90d1bff9ad859863a6a7324bffd75603f1247b38b1b6b9`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56f366246440a01af255c8653a35ec73c718160d30d24532ddef7bf179d826`  
		Last Modified: Mon, 22 Feb 2021 23:03:14 GMT  
		Size: 84.6 MB (84630606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277679070e81c5f1c2e0f4f6867057b442bcf3c8f8934c366c957e39a56c9506`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24665aa55fbb701500b33fba88fa3535bcb91942d0ece77a3ba7891c597837a`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.18-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4afbf91d452ffd2ba54be842a1a4b7d43c5ccbec19f8ab06f04a588b3806371c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132601058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296be39e4a521d5333ea340c6f961db79b331ff95706ab04d4e6259cbd6cc0e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:59:02 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 23:27:31 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 23:27:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:32:43 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:32:51 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:32:55 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:33:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:33:32 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:33:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028e2c33df93b6273c68e3ee47798c813fc1dfec069d9f7026f42da2d00bab1`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704db790ada8d22d0f8b7cc92f07cbe3189530818d890574cdbeac376df7c104`  
		Last Modified: Mon, 22 Feb 2021 23:48:48 GMT  
		Size: 90.1 MB (90116019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3480e0e5f746ea13135811926708c0265082b91c0ae12683d1747190fb5847`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eaeed5ac21d3ea1002610bdc4f4811cec9a0eb173406edc042f505622b39ee`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:32270ca5ee62505b8bd83e067e2626d593bec0560bcd4a60e434217089d7ee6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:b519bfc7b05083f03022b11c7a37c2695da7ca3722494864ee38e2ca75dd823c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122219654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891015ba0a338897130cad7372ed9f00fcf77b7b7994b1d08bdaa5c53e831b84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:49 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 23:22:58 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 23:22:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:23:28 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:23:28 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:23:28 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:23:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:23:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:23:30 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:23:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb9a01d184e1cd0cd08617495ad1c00af608b11ed14a1aee9754a4e05368532`  
		Last Modified: Mon, 22 Feb 2021 23:26:09 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde85630a882d56d9e2de097ffc514022b495298f16bef8f8720ee551882ed2`  
		Last Modified: Mon, 22 Feb 2021 23:26:26 GMT  
		Size: 85.6 MB (85558093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24a97a3b501e62738d8a0e12578e43822ea4967d60298dd2506c0339bd52d0c`  
		Last Modified: Mon, 22 Feb 2021 23:26:08 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca65e5a3bb7246d40b27cb04d040b40cf2e04ca3212774f20649b2d54461ead`  
		Last Modified: Mon, 22 Feb 2021 23:26:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6a2a842442924080424f2f1ee93456ba2e164b6e82b60e2889873ca196fe02b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119803703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8500688c5aadb99309719909ca2270d850e0f5164880d402602fa462c93e7590`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:41:23 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 22:57:51 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 22:57:53 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:58:39 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:58:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:58:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 22:58:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:58:43 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:58:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f68101bda465d0def90d1bff9ad859863a6a7324bffd75603f1247b38b1b6b9`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56f366246440a01af255c8653a35ec73c718160d30d24532ddef7bf179d826`  
		Last Modified: Mon, 22 Feb 2021 23:03:14 GMT  
		Size: 84.6 MB (84630606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277679070e81c5f1c2e0f4f6867057b442bcf3c8f8934c366c957e39a56c9506`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 5.0 KB (5034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24665aa55fbb701500b33fba88fa3535bcb91942d0ece77a3ba7891c597837a`  
		Last Modified: Mon, 22 Feb 2021 23:02:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:4afbf91d452ffd2ba54be842a1a4b7d43c5ccbec19f8ab06f04a588b3806371c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132601058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296be39e4a521d5333ea340c6f961db79b331ff95706ab04d4e6259cbd6cc0e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:59:02 GMT
ENV MARIADB_MAJOR=10.4
# Mon, 22 Feb 2021 23:27:31 GMT
ENV MARIADB_VERSION=1:10.4.18+maria~focal
# Mon, 22 Feb 2021 23:27:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:32:43 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:32:51 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:32:55 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:33:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 22 Feb 2021 23:33:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:33:32 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:33:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3028e2c33df93b6273c68e3ee47798c813fc1dfec069d9f7026f42da2d00bab1`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704db790ada8d22d0f8b7cc92f07cbe3189530818d890574cdbeac376df7c104`  
		Last Modified: Mon, 22 Feb 2021 23:48:48 GMT  
		Size: 90.1 MB (90116019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3480e0e5f746ea13135811926708c0265082b91c0ae12683d1747190fb5847`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eaeed5ac21d3ea1002610bdc4f4811cec9a0eb173406edc042f505622b39ee`  
		Last Modified: Mon, 22 Feb 2021 23:48:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:a13b01d9af44097efeca7a3808a524c8052870e59a1eeef074857ba01e70c1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:d866e756c68fce525419ee27e1d76a874c54072e49dfd591891acd28f95760fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124234067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e69b4a7bda8206563d333112c11de8f043815f996d896afae748c977306746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:22:12 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:22:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:22:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:22:52 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:22:52 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:22:53 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:22:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c59f9e205048d588bf0348ecfadb4ae9c1129ba81f8aedf720fd3446408ff`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa441240c225aa867489089e770da81a847b66e18c1cf5bddb79f7e2c8400e4`  
		Last Modified: Mon, 22 Feb 2021 23:25:57 GMT  
		Size: 87.6 MB (87572628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fee6e1dead96fa856d7afa714bd0d4f2eacb5e3822ea519890a7084837be52`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:eacab2a85f2692a71bbecec0ec1d4eab0a813409bc4760b2d15269b05aa2bafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121825675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d6819532a366f80a8a12c2f9e4ba95c2de67748fce8fc06ce32c95095f896d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:40:27 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 22:56:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 22:56:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:57:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:57:40 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:57:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:57:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:57:42 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:57:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29485c9b3cd7eb629c66e8b4a0c8fb3ebb2aa9d2e840e03c64e50087e27ae68`  
		Last Modified: Mon, 22 Feb 2021 23:02:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73aa765ec3b0d56d75bf82710cf3630aeb5f2d43d953ee4e846a3e729d5360`  
		Last Modified: Mon, 22 Feb 2021 23:02:32 GMT  
		Size: 86.7 MB (86652702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e7e791fe18cdc43a40a9a092228efabefe76675de202cbb4a11810b9a452f5`  
		Last Modified: Mon, 22 Feb 2021 23:02:09 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:579b94998b567c524563c8eb2ce1a995f626c363c4ebcce4e0f76c6ebeb4d433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e61642b22fa5ad1b5375824f6906cb9be6ed44ce44598c8c38a76ad7547341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:40 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:16:43 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:16:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:26:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:26:37 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:26:41 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:26:58 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9408f76f8efc8cd4e636b1149ae5c0000b07e0c008aef9453414b7467eb3886`  
		Last Modified: Mon, 22 Feb 2021 23:47:40 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e97e4b9d88b8ee80ced97b5cd60b0e70dfa733e30f855d2395cc43295224fe`  
		Last Modified: Mon, 22 Feb 2021 23:48:00 GMT  
		Size: 92.2 MB (92197515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f1911e37adab2eb549dd7070427a998202609efd248bb17eb0118a0ae2132c`  
		Last Modified: Mon, 22 Feb 2021 23:47:39 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.9`

```console
$ docker pull mariadb@sha256:a13b01d9af44097efeca7a3808a524c8052870e59a1eeef074857ba01e70c1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.9` - linux; amd64

```console
$ docker pull mariadb@sha256:d866e756c68fce525419ee27e1d76a874c54072e49dfd591891acd28f95760fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124234067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e69b4a7bda8206563d333112c11de8f043815f996d896afae748c977306746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:22:12 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:22:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:22:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:22:52 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:22:52 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:22:53 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:22:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c59f9e205048d588bf0348ecfadb4ae9c1129ba81f8aedf720fd3446408ff`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa441240c225aa867489089e770da81a847b66e18c1cf5bddb79f7e2c8400e4`  
		Last Modified: Mon, 22 Feb 2021 23:25:57 GMT  
		Size: 87.6 MB (87572628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fee6e1dead96fa856d7afa714bd0d4f2eacb5e3822ea519890a7084837be52`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:eacab2a85f2692a71bbecec0ec1d4eab0a813409bc4760b2d15269b05aa2bafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121825675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d6819532a366f80a8a12c2f9e4ba95c2de67748fce8fc06ce32c95095f896d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:40:27 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 22:56:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 22:56:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:57:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:57:40 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:57:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:57:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:57:42 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:57:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29485c9b3cd7eb629c66e8b4a0c8fb3ebb2aa9d2e840e03c64e50087e27ae68`  
		Last Modified: Mon, 22 Feb 2021 23:02:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73aa765ec3b0d56d75bf82710cf3630aeb5f2d43d953ee4e846a3e729d5360`  
		Last Modified: Mon, 22 Feb 2021 23:02:32 GMT  
		Size: 86.7 MB (86652702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e7e791fe18cdc43a40a9a092228efabefe76675de202cbb4a11810b9a452f5`  
		Last Modified: Mon, 22 Feb 2021 23:02:09 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9` - linux; ppc64le

```console
$ docker pull mariadb@sha256:579b94998b567c524563c8eb2ce1a995f626c363c4ebcce4e0f76c6ebeb4d433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e61642b22fa5ad1b5375824f6906cb9be6ed44ce44598c8c38a76ad7547341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:40 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:16:43 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:16:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:26:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:26:37 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:26:41 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:26:58 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9408f76f8efc8cd4e636b1149ae5c0000b07e0c008aef9453414b7467eb3886`  
		Last Modified: Mon, 22 Feb 2021 23:47:40 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e97e4b9d88b8ee80ced97b5cd60b0e70dfa733e30f855d2395cc43295224fe`  
		Last Modified: Mon, 22 Feb 2021 23:48:00 GMT  
		Size: 92.2 MB (92197515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f1911e37adab2eb549dd7070427a998202609efd248bb17eb0118a0ae2132c`  
		Last Modified: Mon, 22 Feb 2021 23:47:39 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.9-focal`

```console
$ docker pull mariadb@sha256:a13b01d9af44097efeca7a3808a524c8052870e59a1eeef074857ba01e70c1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.9-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d866e756c68fce525419ee27e1d76a874c54072e49dfd591891acd28f95760fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124234067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e69b4a7bda8206563d333112c11de8f043815f996d896afae748c977306746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:22:12 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:22:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:22:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:22:52 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:22:52 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:22:53 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:22:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c59f9e205048d588bf0348ecfadb4ae9c1129ba81f8aedf720fd3446408ff`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa441240c225aa867489089e770da81a847b66e18c1cf5bddb79f7e2c8400e4`  
		Last Modified: Mon, 22 Feb 2021 23:25:57 GMT  
		Size: 87.6 MB (87572628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fee6e1dead96fa856d7afa714bd0d4f2eacb5e3822ea519890a7084837be52`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:eacab2a85f2692a71bbecec0ec1d4eab0a813409bc4760b2d15269b05aa2bafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121825675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d6819532a366f80a8a12c2f9e4ba95c2de67748fce8fc06ce32c95095f896d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:40:27 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 22:56:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 22:56:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:57:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:57:40 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:57:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:57:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:57:42 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:57:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29485c9b3cd7eb629c66e8b4a0c8fb3ebb2aa9d2e840e03c64e50087e27ae68`  
		Last Modified: Mon, 22 Feb 2021 23:02:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73aa765ec3b0d56d75bf82710cf3630aeb5f2d43d953ee4e846a3e729d5360`  
		Last Modified: Mon, 22 Feb 2021 23:02:32 GMT  
		Size: 86.7 MB (86652702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e7e791fe18cdc43a40a9a092228efabefe76675de202cbb4a11810b9a452f5`  
		Last Modified: Mon, 22 Feb 2021 23:02:09 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.9-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:579b94998b567c524563c8eb2ce1a995f626c363c4ebcce4e0f76c6ebeb4d433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e61642b22fa5ad1b5375824f6906cb9be6ed44ce44598c8c38a76ad7547341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:40 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:16:43 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:16:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:26:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:26:37 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:26:41 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:26:58 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9408f76f8efc8cd4e636b1149ae5c0000b07e0c008aef9453414b7467eb3886`  
		Last Modified: Mon, 22 Feb 2021 23:47:40 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e97e4b9d88b8ee80ced97b5cd60b0e70dfa733e30f855d2395cc43295224fe`  
		Last Modified: Mon, 22 Feb 2021 23:48:00 GMT  
		Size: 92.2 MB (92197515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f1911e37adab2eb549dd7070427a998202609efd248bb17eb0118a0ae2132c`  
		Last Modified: Mon, 22 Feb 2021 23:47:39 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:a13b01d9af44097efeca7a3808a524c8052870e59a1eeef074857ba01e70c1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d866e756c68fce525419ee27e1d76a874c54072e49dfd591891acd28f95760fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124234067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e69b4a7bda8206563d333112c11de8f043815f996d896afae748c977306746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:22:12 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:22:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:22:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:22:52 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:22:52 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:22:53 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:22:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c59f9e205048d588bf0348ecfadb4ae9c1129ba81f8aedf720fd3446408ff`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa441240c225aa867489089e770da81a847b66e18c1cf5bddb79f7e2c8400e4`  
		Last Modified: Mon, 22 Feb 2021 23:25:57 GMT  
		Size: 87.6 MB (87572628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fee6e1dead96fa856d7afa714bd0d4f2eacb5e3822ea519890a7084837be52`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:eacab2a85f2692a71bbecec0ec1d4eab0a813409bc4760b2d15269b05aa2bafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121825675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d6819532a366f80a8a12c2f9e4ba95c2de67748fce8fc06ce32c95095f896d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:40:27 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 22:56:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 22:56:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:57:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:57:40 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:57:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:57:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:57:42 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:57:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29485c9b3cd7eb629c66e8b4a0c8fb3ebb2aa9d2e840e03c64e50087e27ae68`  
		Last Modified: Mon, 22 Feb 2021 23:02:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73aa765ec3b0d56d75bf82710cf3630aeb5f2d43d953ee4e846a3e729d5360`  
		Last Modified: Mon, 22 Feb 2021 23:02:32 GMT  
		Size: 86.7 MB (86652702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e7e791fe18cdc43a40a9a092228efabefe76675de202cbb4a11810b9a452f5`  
		Last Modified: Mon, 22 Feb 2021 23:02:09 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:579b94998b567c524563c8eb2ce1a995f626c363c4ebcce4e0f76c6ebeb4d433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e61642b22fa5ad1b5375824f6906cb9be6ed44ce44598c8c38a76ad7547341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:40 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:16:43 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:16:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:26:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:26:37 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:26:41 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:26:58 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9408f76f8efc8cd4e636b1149ae5c0000b07e0c008aef9453414b7467eb3886`  
		Last Modified: Mon, 22 Feb 2021 23:47:40 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e97e4b9d88b8ee80ced97b5cd60b0e70dfa733e30f855d2395cc43295224fe`  
		Last Modified: Mon, 22 Feb 2021 23:48:00 GMT  
		Size: 92.2 MB (92197515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f1911e37adab2eb549dd7070427a998202609efd248bb17eb0118a0ae2132c`  
		Last Modified: Mon, 22 Feb 2021 23:47:39 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:a13b01d9af44097efeca7a3808a524c8052870e59a1eeef074857ba01e70c1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d866e756c68fce525419ee27e1d76a874c54072e49dfd591891acd28f95760fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124234067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e69b4a7bda8206563d333112c11de8f043815f996d896afae748c977306746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:22:12 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:22:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:22:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:22:52 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:22:52 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:22:53 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:22:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c59f9e205048d588bf0348ecfadb4ae9c1129ba81f8aedf720fd3446408ff`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa441240c225aa867489089e770da81a847b66e18c1cf5bddb79f7e2c8400e4`  
		Last Modified: Mon, 22 Feb 2021 23:25:57 GMT  
		Size: 87.6 MB (87572628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fee6e1dead96fa856d7afa714bd0d4f2eacb5e3822ea519890a7084837be52`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:eacab2a85f2692a71bbecec0ec1d4eab0a813409bc4760b2d15269b05aa2bafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121825675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d6819532a366f80a8a12c2f9e4ba95c2de67748fce8fc06ce32c95095f896d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:40:27 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 22:56:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 22:56:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:57:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:57:40 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:57:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:57:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:57:42 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:57:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29485c9b3cd7eb629c66e8b4a0c8fb3ebb2aa9d2e840e03c64e50087e27ae68`  
		Last Modified: Mon, 22 Feb 2021 23:02:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73aa765ec3b0d56d75bf82710cf3630aeb5f2d43d953ee4e846a3e729d5360`  
		Last Modified: Mon, 22 Feb 2021 23:02:32 GMT  
		Size: 86.7 MB (86652702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e7e791fe18cdc43a40a9a092228efabefe76675de202cbb4a11810b9a452f5`  
		Last Modified: Mon, 22 Feb 2021 23:02:09 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:579b94998b567c524563c8eb2ce1a995f626c363c4ebcce4e0f76c6ebeb4d433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e61642b22fa5ad1b5375824f6906cb9be6ed44ce44598c8c38a76ad7547341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:40 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:16:43 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:16:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:26:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:26:37 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:26:41 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:26:58 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9408f76f8efc8cd4e636b1149ae5c0000b07e0c008aef9453414b7467eb3886`  
		Last Modified: Mon, 22 Feb 2021 23:47:40 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e97e4b9d88b8ee80ced97b5cd60b0e70dfa733e30f855d2395cc43295224fe`  
		Last Modified: Mon, 22 Feb 2021 23:48:00 GMT  
		Size: 92.2 MB (92197515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f1911e37adab2eb549dd7070427a998202609efd248bb17eb0118a0ae2132c`  
		Last Modified: Mon, 22 Feb 2021 23:47:39 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:a13b01d9af44097efeca7a3808a524c8052870e59a1eeef074857ba01e70c1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:d866e756c68fce525419ee27e1d76a874c54072e49dfd591891acd28f95760fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124234067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e69b4a7bda8206563d333112c11de8f043815f996d896afae748c977306746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:22:12 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:22:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:22:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:22:52 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:22:52 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:22:53 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:22:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c59f9e205048d588bf0348ecfadb4ae9c1129ba81f8aedf720fd3446408ff`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa441240c225aa867489089e770da81a847b66e18c1cf5bddb79f7e2c8400e4`  
		Last Modified: Mon, 22 Feb 2021 23:25:57 GMT  
		Size: 87.6 MB (87572628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fee6e1dead96fa856d7afa714bd0d4f2eacb5e3822ea519890a7084837be52`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:eacab2a85f2692a71bbecec0ec1d4eab0a813409bc4760b2d15269b05aa2bafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121825675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d6819532a366f80a8a12c2f9e4ba95c2de67748fce8fc06ce32c95095f896d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:40:27 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 22:56:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 22:56:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:57:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:57:40 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:57:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:57:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:57:42 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:57:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29485c9b3cd7eb629c66e8b4a0c8fb3ebb2aa9d2e840e03c64e50087e27ae68`  
		Last Modified: Mon, 22 Feb 2021 23:02:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73aa765ec3b0d56d75bf82710cf3630aeb5f2d43d953ee4e846a3e729d5360`  
		Last Modified: Mon, 22 Feb 2021 23:02:32 GMT  
		Size: 86.7 MB (86652702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e7e791fe18cdc43a40a9a092228efabefe76675de202cbb4a11810b9a452f5`  
		Last Modified: Mon, 22 Feb 2021 23:02:09 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:579b94998b567c524563c8eb2ce1a995f626c363c4ebcce4e0f76c6ebeb4d433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e61642b22fa5ad1b5375824f6906cb9be6ed44ce44598c8c38a76ad7547341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:40 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:16:43 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:16:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:26:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:26:37 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:26:41 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:26:58 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9408f76f8efc8cd4e636b1149ae5c0000b07e0c008aef9453414b7467eb3886`  
		Last Modified: Mon, 22 Feb 2021 23:47:40 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e97e4b9d88b8ee80ced97b5cd60b0e70dfa733e30f855d2395cc43295224fe`  
		Last Modified: Mon, 22 Feb 2021 23:48:00 GMT  
		Size: 92.2 MB (92197515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f1911e37adab2eb549dd7070427a998202609efd248bb17eb0118a0ae2132c`  
		Last Modified: Mon, 22 Feb 2021 23:47:39 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:a13b01d9af44097efeca7a3808a524c8052870e59a1eeef074857ba01e70c1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:d866e756c68fce525419ee27e1d76a874c54072e49dfd591891acd28f95760fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124234067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e69b4a7bda8206563d333112c11de8f043815f996d896afae748c977306746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:38:20 GMT
ADD file:2a90223d9f00d31e31eff6b207c57af4b7d27276195b94bec991457a6998180c in / 
# Thu, 21 Jan 2021 03:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:38:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:38:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:38:23 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 11:57:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 11:57:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:57:52 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 11:58:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 11:58:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 11:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 11:58:08 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 11:58:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:22:12 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:22:13 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:22:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:22:52 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:22:52 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:22:53 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:22:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:83ee3a23efb7c75849515a6d46551c608b255d8402a4d3753752b88e0dc188fa`  
		Last Modified: Thu, 21 Jan 2021 03:40:40 GMT  
		Size: 28.6 MB (28565893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db98fc6f11f08950985a203e07755c3262c680d00084f601e7304b768c83b3b1`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f611acd52c6cad803b06b5ba932e4aabd0f2d0d5a4d050c81de2832fcb781274`  
		Last Modified: Thu, 21 Jan 2021 03:40:35 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2333e25466a634bfafc30b42f755d5c4deb9cbb8fab2ae9b892f36abb67f78`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ac4b825fd73c33c1174d9439b607718992fae80dd7e88b4ad459f2fcaf443`  
		Last Modified: Thu, 21 Jan 2021 12:02:53 GMT  
		Size: 5.5 MB (5488704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20afcf9b05533a50381d1cfd8764c1a788f0a9a06cd07e82ae0932c2431dc08`  
		Last Modified: Thu, 21 Jan 2021 12:02:52 GMT  
		Size: 1.3 MB (1324672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5dc6dcf1937aa1b8b1d8fa6ece04dbf357900e49e7a926ab07a34ae8cd0b2`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c71d744483a6fa166a97940a0ce1f93fbdeb109bbc406201effa7c144a51c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:51 GMT  
		Size: 1.3 MB (1271454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a8cc01d1ce8380af8bbf769bccb59830f89db337f2c62cb04353a51b0193f`  
		Last Modified: Thu, 21 Jan 2021 12:02:49 GMT  
		Size: 2.5 KB (2488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c59f9e205048d588bf0348ecfadb4ae9c1129ba81f8aedf720fd3446408ff`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa441240c225aa867489089e770da81a847b66e18c1cf5bddb79f7e2c8400e4`  
		Last Modified: Mon, 22 Feb 2021 23:25:57 GMT  
		Size: 87.6 MB (87572628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fee6e1dead96fa856d7afa714bd0d4f2eacb5e3822ea519890a7084837be52`  
		Last Modified: Mon, 22 Feb 2021 23:25:39 GMT  
		Size: 5.0 KB (5032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:eacab2a85f2692a71bbecec0ec1d4eab0a813409bc4760b2d15269b05aa2bafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121825675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8d6819532a366f80a8a12c2f9e4ba95c2de67748fce8fc06ce32c95095f896d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:49:52 GMT
ADD file:545034ea3827af1e798fe258a2c4b8bb8fb5badc040b6003de9523eb395fa271 in / 
# Thu, 21 Jan 2021 03:49:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:49:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:49:59 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:00 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:39:36 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:39:52 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:39:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:40:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:40:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:40:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:40:24 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:40:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:40:27 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 22:56:45 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 22:56:48 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 22:57:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 22:57:40 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 22:57:40 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 22:57:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 22:57:42 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 22:57:43 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:19d658f3801a0fe0a5260f829f7f2d04d9153f1fc8556771ddbb5a672fa91aad`  
		Last Modified: Tue, 19 Jan 2021 08:25:38 GMT  
		Size: 27.2 MB (27172933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bdea3dddb14aaf7dfe4ed67963d3c95d1325f4c5b8da5b9d6febaf9df6d875`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0c92402f48f37a5d3bf1b351e5c6cbed6cec502dc9138f974a2e114c29ce4`  
		Last Modified: Thu, 21 Jan 2021 03:52:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b7d6f5e8d5e6798d5a292864880dff365e2942d95376ff609c1e916988569`  
		Last Modified: Thu, 21 Jan 2021 05:47:08 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4309d7b0e4d6fd55d9f0e73656707ec9113fa99dd583b3935275c6cace298`  
		Last Modified: Thu, 21 Jan 2021 05:47:10 GMT  
		Size: 5.5 MB (5456508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9947f6df950e3176936d1b2ce059122ae077f90f154470e287d5a63f97255590`  
		Last Modified: Thu, 21 Jan 2021 05:47:09 GMT  
		Size: 1.3 MB (1261886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875e2be5d265eb66b81430a94ae317145292da3e8f462c8212d22228522e5005`  
		Last Modified: Thu, 21 Jan 2021 05:47:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223795b422204535226226d07a28f273d181d1a8e10968fcfaff86965fef309e`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 1.3 MB (1270864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc657677ae3e0889cf4b2d2f583ae2afff1e044699f2ef9efa09e3c11f3b6a`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29485c9b3cd7eb629c66e8b4a0c8fb3ebb2aa9d2e840e03c64e50087e27ae68`  
		Last Modified: Mon, 22 Feb 2021 23:02:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73aa765ec3b0d56d75bf82710cf3630aeb5f2d43d953ee4e846a3e729d5360`  
		Last Modified: Mon, 22 Feb 2021 23:02:32 GMT  
		Size: 86.7 MB (86652702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e7e791fe18cdc43a40a9a092228efabefe76675de202cbb4a11810b9a452f5`  
		Last Modified: Mon, 22 Feb 2021 23:02:09 GMT  
		Size: 5.0 KB (5031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:579b94998b567c524563c8eb2ce1a995f626c363c4ebcce4e0f76c6ebeb4d433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134682433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e61642b22fa5ad1b5375824f6906cb9be6ed44ce44598c8c38a76ad7547341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 21 Jan 2021 03:50:20 GMT
ADD file:49b5be3021a4fb821776e6f80319442aec170cc102d0a654d693b5454690c821 in / 
# Thu, 21 Jan 2021 03:50:30 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:50:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 03:50:50 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:50:54 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:51:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 21 Jan 2021 05:52:54 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:52:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 21 Jan 2021 05:53:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Jan 2021 05:53:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Jan 2021 05:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:54:29 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 21 Jan 2021 05:54:37 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Jan 2021 05:54:40 GMT
ENV MARIADB_MAJOR=10.5
# Mon, 22 Feb 2021 23:16:43 GMT
ENV MARIADB_VERSION=1:10.5.9+maria~focal
# Mon, 22 Feb 2021 23:16:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Mon, 22 Feb 2021 23:26:24 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Mon, 22 Feb 2021 23:26:37 GMT
VOLUME [/var/lib/mysql]
# Mon, 22 Feb 2021 23:26:41 GMT
COPY file:52b881219ebb536dc2a07a100dc6c7e2307319ab3fee74c26c69db394fbb63eb in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:26:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:26:58 GMT
EXPOSE 3306
# Mon, 22 Feb 2021 23:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ed91c6e011d4ed173552e8b28be61b946656c0330984b66bbbafa1f5e34f7fda`  
		Last Modified: Thu, 21 Jan 2021 03:55:01 GMT  
		Size: 33.3 MB (33280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906af84ca057c8c6651f31329207a1be8db5730495704aa9e38333d794bd3d4`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3169ead309f6248d857e6e5c4891d40de8b742b21729c03d465aff49558d9135`  
		Last Modified: Thu, 21 Jan 2021 03:54:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:118d20346f2cbcc567a584e73420ee046c014e5274292b98c726e7e607f2498d`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9c9e7cf1141ba6332b38044a197572f922ee6692648d4ffe85b72a568b8151`  
		Last Modified: Thu, 21 Jan 2021 06:23:23 GMT  
		Size: 6.7 MB (6668825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df79a7d52519083ad69280dfe954a5278b23e97d632efa62b28f3112fc174f3`  
		Last Modified: Thu, 21 Jan 2021 06:23:24 GMT  
		Size: 1.2 MB (1244330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9785f186be73d26aa25b400789a8607f7a0c9dacc3ca292ca58140c9b301f326`  
		Last Modified: Thu, 21 Jan 2021 06:23:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab568b951c4872ed3d7c6f58092adb0768c36a54bf35cf4afb2354538440d52f`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 1.3 MB (1280957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f095c9f1176a6c008962edea812b5ff6548bd724504e6df3f38d7ceef3845c52`  
		Last Modified: Thu, 21 Jan 2021 06:23:17 GMT  
		Size: 2.5 KB (2492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9408f76f8efc8cd4e636b1149ae5c0000b07e0c008aef9453414b7467eb3886`  
		Last Modified: Mon, 22 Feb 2021 23:47:40 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e97e4b9d88b8ee80ced97b5cd60b0e70dfa733e30f855d2395cc43295224fe`  
		Last Modified: Mon, 22 Feb 2021 23:48:00 GMT  
		Size: 92.2 MB (92197515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f1911e37adab2eb549dd7070427a998202609efd248bb17eb0118a0ae2132c`  
		Last Modified: Mon, 22 Feb 2021 23:47:39 GMT  
		Size: 5.0 KB (5035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
