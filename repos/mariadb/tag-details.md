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
$ docker pull mariadb@sha256:8040983db146f729749081c6b216a19d52e0973134e2e34c0b4fd87f48bc15b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:03fb19fa5729856ec8c8ed23d421ed1ab6c0e2d63fdf2b1bd8d311025e228a9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125593666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade39f0469a3fa0e5f907e4dd7861a4e77573b0757bd4055a7b4c52baea58590`
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
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 11:58:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:58:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:58:39 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:58:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:58:39 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:58:39 GMT
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
	-	`sha256:5d1a793b093fb66b368496d9fc031d57477617a83485edd703c254af153a8e92`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477cd2b3eba82e02507024ebdc4dee18f00503fca5308d5d4258dc1a2fd29741`  
		Last Modified: Thu, 21 Jan 2021 12:03:06 GMT  
		Size: 88.9 MB (88932340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40245454316697c87c982e323046c544d7838a1758bf9f85b8fdc0de8e8cf4c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c892a2d0194f19d0aa29fa165cdbfeb6be619cbf68b7a9f715369f7f08c05311
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123207507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3ab601101c5c8e7e2238bb43637af4113de1d73fea960e84f06a91663ad364`
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
# Thu, 21 Jan 2021 05:40:28 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:40:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:41:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:41:05 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:41:06 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:41:07 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:41:08 GMT
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
	-	`sha256:01b09912c33f2e7b6a76320f2c201590899ee9b65c0a74c459e877702bbed84f`  
		Last Modified: Thu, 21 Jan 2021 05:47:04 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bd2c4c297c8d6742d93d7dcd7fa909f85e44eb27209214b362fc52f48a1d48`  
		Last Modified: Thu, 21 Jan 2021 05:47:29 GMT  
		Size: 88.0 MB (88034645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c6e38659e4a0759fb2b50eb8fa140f50e1abdc8038bb5cb07209c908d80fca`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:998603c1d9d5ce3c30340897c9071dfaac88b3b8bedf1c351d207dfdad99a401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135593595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd15ad097e80bfded8f3563be92ffefc5e426a4f65a5b3b4d3ea04f6c44c07a`
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
# Thu, 21 Jan 2021 05:54:46 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:54:58 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:58:16 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:58:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:58:31 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:58:40 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:58:44 GMT
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
	-	`sha256:d17dc5940401537ceb8f16e75f7b3e24ed0227778aa65a34487ed355ec81b5a8`  
		Last Modified: Thu, 21 Jan 2021 06:23:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6539b7b968359217718b2cfdc33635f618728f4db73eff20f977cc203783b`  
		Last Modified: Thu, 21 Jan 2021 06:23:42 GMT  
		Size: 93.1 MB (93108795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412f01454a1c306983d7b46c8dca3ae6d371cd540b7d3be8cf70d8b891f8b432`  
		Last Modified: Thu, 21 Jan 2021 06:23:18 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1`

```console
$ docker pull mariadb@sha256:78ed2b896632023880a6ae9bb0b4523c25e91fa8833f4918d5314ac3fdb6dc3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1` - linux; amd64

```console
$ docker pull mariadb@sha256:90cb7c01db5b7889b23dc195468e0e20bba166a90c09286ebb3a1831d0fe4fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113175153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce131c51a9ffe75ba064383cce7a657a3871fd599693c7742230e85b06adc2c`
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
# Thu, 21 Jan 2021 12:02:15 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 12:02:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 12:02:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 12:02:16 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 12:02:16 GMT
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
	-	`sha256:fcb7efdd020922298a5589ca3131e17d468d4c924b9c723d29583001c3e95cc0`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039e9c1ea196f89eaa7ef120e3534921e35e972870b0746c5b2e1e28ef0e6b4`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dbbd61f795c88c7a3e53a06df14a4a1e87d988b2122ec8891b128adbecd1f377
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105800356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbf64ce6fcaabba048cb32d850e4fd905d916aba93c835fcd955541566bcb47`
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
# Thu, 21 Jan 2021 05:46:23 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:46:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:46:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:46:26 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:46:27 GMT
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
	-	`sha256:461b349c0f8d8e4bbaca6d0e147d5eb0b376096dd3e25bb581740e2a632a4d5e`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 4.9 KB (4920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1573498239a4062cec96bec5d6fd7d452ba33e733efeeee0241a3ccd6687c2c5`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a0efc73feaef5697a7dbe2cbc55b39c4a3faa4dc4fae35e341af748ff730ce5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9553325ad04a340fdff3efebe1376243017d23d115f6bfcb81ad8cd439c90d3`
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
# Thu, 21 Jan 2021 06:22:18 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:22:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:22:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:22:36 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:22:41 GMT
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
	-	`sha256:5e9813ec4839cc54540847d201b0eb44bf677395ed1cdfceb38c5f936fe2864c`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204f53aaeb252dfea54031125f0c686ec7b6cf23ee71099c84734dd7e7ae8c8`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48`

```console
$ docker pull mariadb@sha256:78ed2b896632023880a6ae9bb0b4523c25e91fa8833f4918d5314ac3fdb6dc3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48` - linux; amd64

```console
$ docker pull mariadb@sha256:90cb7c01db5b7889b23dc195468e0e20bba166a90c09286ebb3a1831d0fe4fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113175153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce131c51a9ffe75ba064383cce7a657a3871fd599693c7742230e85b06adc2c`
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
# Thu, 21 Jan 2021 12:02:15 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 12:02:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 12:02:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 12:02:16 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 12:02:16 GMT
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
	-	`sha256:fcb7efdd020922298a5589ca3131e17d468d4c924b9c723d29583001c3e95cc0`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039e9c1ea196f89eaa7ef120e3534921e35e972870b0746c5b2e1e28ef0e6b4`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dbbd61f795c88c7a3e53a06df14a4a1e87d988b2122ec8891b128adbecd1f377
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105800356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbf64ce6fcaabba048cb32d850e4fd905d916aba93c835fcd955541566bcb47`
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
# Thu, 21 Jan 2021 05:46:23 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:46:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:46:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:46:26 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:46:27 GMT
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
	-	`sha256:461b349c0f8d8e4bbaca6d0e147d5eb0b376096dd3e25bb581740e2a632a4d5e`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 4.9 KB (4920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1573498239a4062cec96bec5d6fd7d452ba33e733efeeee0241a3ccd6687c2c5`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a0efc73feaef5697a7dbe2cbc55b39c4a3faa4dc4fae35e341af748ff730ce5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9553325ad04a340fdff3efebe1376243017d23d115f6bfcb81ad8cd439c90d3`
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
# Thu, 21 Jan 2021 06:22:18 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:22:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:22:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:22:36 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:22:41 GMT
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
	-	`sha256:5e9813ec4839cc54540847d201b0eb44bf677395ed1cdfceb38c5f936fe2864c`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204f53aaeb252dfea54031125f0c686ec7b6cf23ee71099c84734dd7e7ae8c8`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.48-bionic`

```console
$ docker pull mariadb@sha256:78ed2b896632023880a6ae9bb0b4523c25e91fa8833f4918d5314ac3fdb6dc3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.48-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:90cb7c01db5b7889b23dc195468e0e20bba166a90c09286ebb3a1831d0fe4fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113175153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce131c51a9ffe75ba064383cce7a657a3871fd599693c7742230e85b06adc2c`
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
# Thu, 21 Jan 2021 12:02:15 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 12:02:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 12:02:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 12:02:16 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 12:02:16 GMT
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
	-	`sha256:fcb7efdd020922298a5589ca3131e17d468d4c924b9c723d29583001c3e95cc0`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039e9c1ea196f89eaa7ef120e3534921e35e972870b0746c5b2e1e28ef0e6b4`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dbbd61f795c88c7a3e53a06df14a4a1e87d988b2122ec8891b128adbecd1f377
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105800356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbf64ce6fcaabba048cb32d850e4fd905d916aba93c835fcd955541566bcb47`
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
# Thu, 21 Jan 2021 05:46:23 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:46:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:46:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:46:26 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:46:27 GMT
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
	-	`sha256:461b349c0f8d8e4bbaca6d0e147d5eb0b376096dd3e25bb581740e2a632a4d5e`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 4.9 KB (4920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1573498239a4062cec96bec5d6fd7d452ba33e733efeeee0241a3ccd6687c2c5`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.48-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a0efc73feaef5697a7dbe2cbc55b39c4a3faa4dc4fae35e341af748ff730ce5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9553325ad04a340fdff3efebe1376243017d23d115f6bfcb81ad8cd439c90d3`
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
# Thu, 21 Jan 2021 06:22:18 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:22:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:22:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:22:36 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:22:41 GMT
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
	-	`sha256:5e9813ec4839cc54540847d201b0eb44bf677395ed1cdfceb38c5f936fe2864c`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204f53aaeb252dfea54031125f0c686ec7b6cf23ee71099c84734dd7e7ae8c8`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1-bionic`

```console
$ docker pull mariadb@sha256:78ed2b896632023880a6ae9bb0b4523c25e91fa8833f4918d5314ac3fdb6dc3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:90cb7c01db5b7889b23dc195468e0e20bba166a90c09286ebb3a1831d0fe4fdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113175153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce131c51a9ffe75ba064383cce7a657a3871fd599693c7742230e85b06adc2c`
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
# Thu, 21 Jan 2021 12:02:15 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 12:02:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 12:02:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 12:02:16 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 12:02:16 GMT
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
	-	`sha256:fcb7efdd020922298a5589ca3131e17d468d4c924b9c723d29583001c3e95cc0`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039e9c1ea196f89eaa7ef120e3534921e35e972870b0746c5b2e1e28ef0e6b4`  
		Last Modified: Thu, 21 Jan 2021 12:04:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:dbbd61f795c88c7a3e53a06df14a4a1e87d988b2122ec8891b128adbecd1f377
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105800356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbf64ce6fcaabba048cb32d850e4fd905d916aba93c835fcd955541566bcb47`
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
# Thu, 21 Jan 2021 05:46:23 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:46:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:46:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:46:26 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:46:27 GMT
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
	-	`sha256:461b349c0f8d8e4bbaca6d0e147d5eb0b376096dd3e25bb581740e2a632a4d5e`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 4.9 KB (4920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1573498239a4062cec96bec5d6fd7d452ba33e733efeeee0241a3ccd6687c2c5`  
		Last Modified: Thu, 21 Jan 2021 05:49:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:a0efc73feaef5697a7dbe2cbc55b39c4a3faa4dc4fae35e341af748ff730ce5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118172431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9553325ad04a340fdff3efebe1376243017d23d115f6bfcb81ad8cd439c90d3`
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
# Thu, 21 Jan 2021 06:22:18 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:22:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:22:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:22:36 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:22:41 GMT
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
	-	`sha256:5e9813ec4839cc54540847d201b0eb44bf677395ed1cdfceb38c5f936fe2864c`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204f53aaeb252dfea54031125f0c686ec7b6cf23ee71099c84734dd7e7ae8c8`  
		Last Modified: Thu, 21 Jan 2021 06:30:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:2e1204e7a83aa1df98fd73d4a93fbd619c417ae8125469934813baf562efe52f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:1eddad06b31f85d650cfbf1e99671204a0f4e1bca48a51e218993a74dd94a75d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109016659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b381bd77f030450bda844da7c3179a8e36ae66cf05714f19644f972aa4f23d`
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
# Thu, 21 Jan 2021 12:00:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 12:00:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 12:01:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 12:01:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 12:01:16 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 12:01:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 12:01:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 12:01:17 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 12:01:17 GMT
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
	-	`sha256:e72905cadd4563e4a859541e9e3531d2c7998164052fc0b30ac935a667b0b88c`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e96e2914e98a25c8bf390dd9d8a0e6cfafec843e09094f8bc7e285f347598`  
		Last Modified: Thu, 21 Jan 2021 12:04:40 GMT  
		Size: 75.2 MB (75223392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a7a7a768daae4e888a94426cc1381a0b41faf8a0cb5133ba43eb88e3e1273a`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74baf1bee3db1e5449a5f12ac4e792e28c924ab26684e7f7f2e40058afe7147`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c2f8c8b7ec560747b9b79121c4c2f4f2a26b86212bf96e92a5e0b3a4fe45bebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104079081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb9d07de25dfcd9e183fe67981ed1071656edd64dd3f517071e622446cd9436`
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
# Thu, 21 Jan 2021 05:44:24 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 05:44:26 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:45:05 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:45:07 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:45:08 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:45:11 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:45:11 GMT
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
	-	`sha256:bd311a57acc06cfb9dc7eefac07890dffad688e9408529bb898dbf829b1899d7`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5cdb7b75191e35c8dac5be475e7156f9491394ac453fbb0ae520e281cd71c5`  
		Last Modified: Thu, 21 Jan 2021 05:49:25 GMT  
		Size: 73.7 MB (73749042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfa5e4158ee54d51fb64f80790fdc77b7ed24bbcf1bf9f4310f551870a0744`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d113e6fc04823fb737e583c4667b019bdac45e817dc8707bc36dd7d079a4f5`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dd886333fbc1382e7ea08dc0b276d68cf82acf33a246f31cc631ae01a962de8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116232184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee93af2d3ba32c8fadbcf3cefc87677ab15ca56aedf6b798580acbe511ebd28a`
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
# Thu, 21 Jan 2021 06:13:15 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 06:13:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:16:49 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:16:59 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:17:01 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:17:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:17:38 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:17:43 GMT
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
	-	`sha256:68fbbbd1a56d11d01bc18ce250bb1ca051610d99a0638228774c8b0ee7919f0e`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eb202bf05d0eae31fb7ebcdd37bbad150fed05d0a1ec604068b336e50d3330`  
		Last Modified: Thu, 21 Jan 2021 06:29:38 GMT  
		Size: 78.0 MB (77983852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47aa3a555e06b48bb64ca46d9d2a2f0628253f830c03638a583d27ab7bd300f5`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14104413d88cd135a47e51e8cb3dd3881245ba0eac232f46a0d689af4708cd4e`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.36`

```console
$ docker pull mariadb@sha256:2e1204e7a83aa1df98fd73d4a93fbd619c417ae8125469934813baf562efe52f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.36` - linux; amd64

```console
$ docker pull mariadb@sha256:1eddad06b31f85d650cfbf1e99671204a0f4e1bca48a51e218993a74dd94a75d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109016659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b381bd77f030450bda844da7c3179a8e36ae66cf05714f19644f972aa4f23d`
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
# Thu, 21 Jan 2021 12:00:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 12:00:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 12:01:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 12:01:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 12:01:16 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 12:01:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 12:01:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 12:01:17 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 12:01:17 GMT
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
	-	`sha256:e72905cadd4563e4a859541e9e3531d2c7998164052fc0b30ac935a667b0b88c`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e96e2914e98a25c8bf390dd9d8a0e6cfafec843e09094f8bc7e285f347598`  
		Last Modified: Thu, 21 Jan 2021 12:04:40 GMT  
		Size: 75.2 MB (75223392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a7a7a768daae4e888a94426cc1381a0b41faf8a0cb5133ba43eb88e3e1273a`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74baf1bee3db1e5449a5f12ac4e792e28c924ab26684e7f7f2e40058afe7147`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.36` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c2f8c8b7ec560747b9b79121c4c2f4f2a26b86212bf96e92a5e0b3a4fe45bebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104079081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb9d07de25dfcd9e183fe67981ed1071656edd64dd3f517071e622446cd9436`
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
# Thu, 21 Jan 2021 05:44:24 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 05:44:26 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:45:05 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:45:07 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:45:08 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:45:11 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:45:11 GMT
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
	-	`sha256:bd311a57acc06cfb9dc7eefac07890dffad688e9408529bb898dbf829b1899d7`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5cdb7b75191e35c8dac5be475e7156f9491394ac453fbb0ae520e281cd71c5`  
		Last Modified: Thu, 21 Jan 2021 05:49:25 GMT  
		Size: 73.7 MB (73749042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfa5e4158ee54d51fb64f80790fdc77b7ed24bbcf1bf9f4310f551870a0744`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d113e6fc04823fb737e583c4667b019bdac45e817dc8707bc36dd7d079a4f5`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.36` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dd886333fbc1382e7ea08dc0b276d68cf82acf33a246f31cc631ae01a962de8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116232184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee93af2d3ba32c8fadbcf3cefc87677ab15ca56aedf6b798580acbe511ebd28a`
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
# Thu, 21 Jan 2021 06:13:15 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 06:13:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:16:49 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:16:59 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:17:01 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:17:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:17:38 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:17:43 GMT
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
	-	`sha256:68fbbbd1a56d11d01bc18ce250bb1ca051610d99a0638228774c8b0ee7919f0e`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eb202bf05d0eae31fb7ebcdd37bbad150fed05d0a1ec604068b336e50d3330`  
		Last Modified: Thu, 21 Jan 2021 06:29:38 GMT  
		Size: 78.0 MB (77983852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47aa3a555e06b48bb64ca46d9d2a2f0628253f830c03638a583d27ab7bd300f5`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14104413d88cd135a47e51e8cb3dd3881245ba0eac232f46a0d689af4708cd4e`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.36-bionic`

```console
$ docker pull mariadb@sha256:2e1204e7a83aa1df98fd73d4a93fbd619c417ae8125469934813baf562efe52f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.36-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:1eddad06b31f85d650cfbf1e99671204a0f4e1bca48a51e218993a74dd94a75d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109016659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b381bd77f030450bda844da7c3179a8e36ae66cf05714f19644f972aa4f23d`
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
# Thu, 21 Jan 2021 12:00:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 12:00:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 12:01:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 12:01:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 12:01:16 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 12:01:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 12:01:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 12:01:17 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 12:01:17 GMT
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
	-	`sha256:e72905cadd4563e4a859541e9e3531d2c7998164052fc0b30ac935a667b0b88c`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e96e2914e98a25c8bf390dd9d8a0e6cfafec843e09094f8bc7e285f347598`  
		Last Modified: Thu, 21 Jan 2021 12:04:40 GMT  
		Size: 75.2 MB (75223392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a7a7a768daae4e888a94426cc1381a0b41faf8a0cb5133ba43eb88e3e1273a`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74baf1bee3db1e5449a5f12ac4e792e28c924ab26684e7f7f2e40058afe7147`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.36-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c2f8c8b7ec560747b9b79121c4c2f4f2a26b86212bf96e92a5e0b3a4fe45bebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104079081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb9d07de25dfcd9e183fe67981ed1071656edd64dd3f517071e622446cd9436`
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
# Thu, 21 Jan 2021 05:44:24 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 05:44:26 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:45:05 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:45:07 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:45:08 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:45:11 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:45:11 GMT
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
	-	`sha256:bd311a57acc06cfb9dc7eefac07890dffad688e9408529bb898dbf829b1899d7`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5cdb7b75191e35c8dac5be475e7156f9491394ac453fbb0ae520e281cd71c5`  
		Last Modified: Thu, 21 Jan 2021 05:49:25 GMT  
		Size: 73.7 MB (73749042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfa5e4158ee54d51fb64f80790fdc77b7ed24bbcf1bf9f4310f551870a0744`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d113e6fc04823fb737e583c4667b019bdac45e817dc8707bc36dd7d079a4f5`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.36-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dd886333fbc1382e7ea08dc0b276d68cf82acf33a246f31cc631ae01a962de8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116232184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee93af2d3ba32c8fadbcf3cefc87677ab15ca56aedf6b798580acbe511ebd28a`
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
# Thu, 21 Jan 2021 06:13:15 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 06:13:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:16:49 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:16:59 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:17:01 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:17:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:17:38 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:17:43 GMT
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
	-	`sha256:68fbbbd1a56d11d01bc18ce250bb1ca051610d99a0638228774c8b0ee7919f0e`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eb202bf05d0eae31fb7ebcdd37bbad150fed05d0a1ec604068b336e50d3330`  
		Last Modified: Thu, 21 Jan 2021 06:29:38 GMT  
		Size: 78.0 MB (77983852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47aa3a555e06b48bb64ca46d9d2a2f0628253f830c03638a583d27ab7bd300f5`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14104413d88cd135a47e51e8cb3dd3881245ba0eac232f46a0d689af4708cd4e`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:2e1204e7a83aa1df98fd73d4a93fbd619c417ae8125469934813baf562efe52f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:1eddad06b31f85d650cfbf1e99671204a0f4e1bca48a51e218993a74dd94a75d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109016659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b381bd77f030450bda844da7c3179a8e36ae66cf05714f19644f972aa4f23d`
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
# Thu, 21 Jan 2021 12:00:43 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 12:00:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 12:01:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 12:01:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 12:01:16 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 12:01:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 12:01:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 12:01:17 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 12:01:17 GMT
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
	-	`sha256:e72905cadd4563e4a859541e9e3531d2c7998164052fc0b30ac935a667b0b88c`  
		Last Modified: Thu, 21 Jan 2021 12:04:27 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e96e2914e98a25c8bf390dd9d8a0e6cfafec843e09094f8bc7e285f347598`  
		Last Modified: Thu, 21 Jan 2021 12:04:40 GMT  
		Size: 75.2 MB (75223392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a7a7a768daae4e888a94426cc1381a0b41faf8a0cb5133ba43eb88e3e1273a`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74baf1bee3db1e5449a5f12ac4e792e28c924ab26684e7f7f2e40058afe7147`  
		Last Modified: Thu, 21 Jan 2021 12:04:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c2f8c8b7ec560747b9b79121c4c2f4f2a26b86212bf96e92a5e0b3a4fe45bebc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104079081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb9d07de25dfcd9e183fe67981ed1071656edd64dd3f517071e622446cd9436`
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
# Thu, 21 Jan 2021 05:44:24 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 05:44:26 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:45:05 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:45:07 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:45:08 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:45:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:45:11 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:45:11 GMT
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
	-	`sha256:bd311a57acc06cfb9dc7eefac07890dffad688e9408529bb898dbf829b1899d7`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5cdb7b75191e35c8dac5be475e7156f9491394ac453fbb0ae520e281cd71c5`  
		Last Modified: Thu, 21 Jan 2021 05:49:25 GMT  
		Size: 73.7 MB (73749042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dfa5e4158ee54d51fb64f80790fdc77b7ed24bbcf1bf9f4310f551870a0744`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d113e6fc04823fb737e583c4667b019bdac45e817dc8707bc36dd7d079a4f5`  
		Last Modified: Thu, 21 Jan 2021 05:49:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:dd886333fbc1382e7ea08dc0b276d68cf82acf33a246f31cc631ae01a962de8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.2 MB (116232184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee93af2d3ba32c8fadbcf3cefc87677ab15ca56aedf6b798580acbe511ebd28a`
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
# Thu, 21 Jan 2021 06:13:15 GMT
ENV MARIADB_VERSION=1:10.2.36+maria~bionic
# Thu, 21 Jan 2021 06:13:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:16:49 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:16:59 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:17:01 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:17:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:17:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:17:38 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:17:43 GMT
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
	-	`sha256:68fbbbd1a56d11d01bc18ce250bb1ca051610d99a0638228774c8b0ee7919f0e`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eb202bf05d0eae31fb7ebcdd37bbad150fed05d0a1ec604068b336e50d3330`  
		Last Modified: Thu, 21 Jan 2021 06:29:38 GMT  
		Size: 78.0 MB (77983852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47aa3a555e06b48bb64ca46d9d2a2f0628253f830c03638a583d27ab7bd300f5`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14104413d88cd135a47e51e8cb3dd3881245ba0eac232f46a0d689af4708cd4e`  
		Last Modified: Thu, 21 Jan 2021 06:29:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:820ef6569f29e76e61bcf0d6005b858037b0f49afddaa7d2943a6c0de646a6d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:3f57f61689aac8c56ebe5d184622c9fa9f0359aad4d481a5f52a74d92534540e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119247331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2abc809aea2acd3c35befc0946d09b6665098615de7b8e860b5df60d67ea396e`
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
# Thu, 21 Jan 2021 11:59:23 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 11:59:24 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:59:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:59:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:59:53 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:59:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 11:59:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:59:54 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:59:54 GMT
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
	-	`sha256:60f77f5f102cf856c02897bbcc07066c00fddbf376423d3d35e870d2894c943e`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce534039c7fd41cb524120e2e9116fac33e6229ea1a9cba14c99a0fda1868ca`  
		Last Modified: Thu, 21 Jan 2021 12:04:14 GMT  
		Size: 82.6 MB (82585884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01014da6acb1ec93717bbd1643af27a01c5a129463fed08abb06c1cc62b3d100`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ffc1a63001f827f81a88e1c5b600dbce98de897f65311296d00b83f4f5cb0a`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6b3f13c88059ae711cd5f74c2cbf17b098541c0277e04c22da87002af9f73d3e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116871767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1912215ebc6c9e79834773575de4b4cf7328f76096c639809f91712acf033d`
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
# Thu, 21 Jan 2021 05:42:21 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 05:42:23 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:43:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:43:09 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:43:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:43:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:43:13 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:43:14 GMT
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
	-	`sha256:30503b1b816b67d95b85a2aa5bb4629030261cdf070f519263adc4cc9b467b94`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2401763c58fae1af4f54b24fb8bcd8ef12c25a573ed6add42c69f46727f1a2ee`  
		Last Modified: Thu, 21 Jan 2021 05:48:53 GMT  
		Size: 81.7 MB (81698789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784582ef68840074e18c294150aac11cdbd3d836587d2d38dc8c81720898d265`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 4.9 KB (4915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b92b5508c1b68482631cefdc59114a74152fb7d29f11516374ae635952b322`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:70c97f38ef062d473d3502708ff31798ca03cfa1aeff6168565a8dd75bf953f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129052717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf901d1f35ca5ea3e90d5415f820d5e973b442a75aaabf6709fb89ff62b7e119`
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
# Thu, 21 Jan 2021 06:03:53 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 06:04:08 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:07:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:07:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:07:58 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:08:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:08:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:08:17 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:08:25 GMT
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
	-	`sha256:10cabac2f70a6357ef272cb67c3cefcf1faa7004bd07f4950fcfaa8039bafa7e`  
		Last Modified: Thu, 21 Jan 2021 06:28:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc0c94895146903b4e9c57d85817555cf21b36e302f7c64e2d6fb05d017b6fd`  
		Last Modified: Thu, 21 Jan 2021 06:28:54 GMT  
		Size: 86.6 MB (86567793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5feb6c8acd8c1db342471fd22b7602f0635fba23a0a37c8d8454065bd5f1f344`  
		Last Modified: Thu, 21 Jan 2021 06:28:37 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21879422024ab16fd75f7d37b8f7b39de729a78e89b16e6a33f0016d9d0b9ed1`  
		Last Modified: Thu, 21 Jan 2021 06:28:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.27`

```console
$ docker pull mariadb@sha256:820ef6569f29e76e61bcf0d6005b858037b0f49afddaa7d2943a6c0de646a6d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.27` - linux; amd64

```console
$ docker pull mariadb@sha256:3f57f61689aac8c56ebe5d184622c9fa9f0359aad4d481a5f52a74d92534540e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119247331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2abc809aea2acd3c35befc0946d09b6665098615de7b8e860b5df60d67ea396e`
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
# Thu, 21 Jan 2021 11:59:23 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 11:59:24 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:59:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:59:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:59:53 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:59:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 11:59:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:59:54 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:59:54 GMT
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
	-	`sha256:60f77f5f102cf856c02897bbcc07066c00fddbf376423d3d35e870d2894c943e`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce534039c7fd41cb524120e2e9116fac33e6229ea1a9cba14c99a0fda1868ca`  
		Last Modified: Thu, 21 Jan 2021 12:04:14 GMT  
		Size: 82.6 MB (82585884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01014da6acb1ec93717bbd1643af27a01c5a129463fed08abb06c1cc62b3d100`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ffc1a63001f827f81a88e1c5b600dbce98de897f65311296d00b83f4f5cb0a`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.27` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6b3f13c88059ae711cd5f74c2cbf17b098541c0277e04c22da87002af9f73d3e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116871767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1912215ebc6c9e79834773575de4b4cf7328f76096c639809f91712acf033d`
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
# Thu, 21 Jan 2021 05:42:21 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 05:42:23 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:43:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:43:09 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:43:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:43:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:43:13 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:43:14 GMT
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
	-	`sha256:30503b1b816b67d95b85a2aa5bb4629030261cdf070f519263adc4cc9b467b94`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2401763c58fae1af4f54b24fb8bcd8ef12c25a573ed6add42c69f46727f1a2ee`  
		Last Modified: Thu, 21 Jan 2021 05:48:53 GMT  
		Size: 81.7 MB (81698789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784582ef68840074e18c294150aac11cdbd3d836587d2d38dc8c81720898d265`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 4.9 KB (4915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b92b5508c1b68482631cefdc59114a74152fb7d29f11516374ae635952b322`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.27` - linux; ppc64le

```console
$ docker pull mariadb@sha256:70c97f38ef062d473d3502708ff31798ca03cfa1aeff6168565a8dd75bf953f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129052717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf901d1f35ca5ea3e90d5415f820d5e973b442a75aaabf6709fb89ff62b7e119`
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
# Thu, 21 Jan 2021 06:03:53 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 06:04:08 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:07:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:07:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:07:58 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:08:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:08:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:08:17 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:08:25 GMT
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
	-	`sha256:10cabac2f70a6357ef272cb67c3cefcf1faa7004bd07f4950fcfaa8039bafa7e`  
		Last Modified: Thu, 21 Jan 2021 06:28:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc0c94895146903b4e9c57d85817555cf21b36e302f7c64e2d6fb05d017b6fd`  
		Last Modified: Thu, 21 Jan 2021 06:28:54 GMT  
		Size: 86.6 MB (86567793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5feb6c8acd8c1db342471fd22b7602f0635fba23a0a37c8d8454065bd5f1f344`  
		Last Modified: Thu, 21 Jan 2021 06:28:37 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21879422024ab16fd75f7d37b8f7b39de729a78e89b16e6a33f0016d9d0b9ed1`  
		Last Modified: Thu, 21 Jan 2021 06:28:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.27-focal`

```console
$ docker pull mariadb@sha256:820ef6569f29e76e61bcf0d6005b858037b0f49afddaa7d2943a6c0de646a6d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.27-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:3f57f61689aac8c56ebe5d184622c9fa9f0359aad4d481a5f52a74d92534540e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119247331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2abc809aea2acd3c35befc0946d09b6665098615de7b8e860b5df60d67ea396e`
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
# Thu, 21 Jan 2021 11:59:23 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 11:59:24 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:59:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:59:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:59:53 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:59:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 11:59:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:59:54 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:59:54 GMT
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
	-	`sha256:60f77f5f102cf856c02897bbcc07066c00fddbf376423d3d35e870d2894c943e`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce534039c7fd41cb524120e2e9116fac33e6229ea1a9cba14c99a0fda1868ca`  
		Last Modified: Thu, 21 Jan 2021 12:04:14 GMT  
		Size: 82.6 MB (82585884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01014da6acb1ec93717bbd1643af27a01c5a129463fed08abb06c1cc62b3d100`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ffc1a63001f827f81a88e1c5b600dbce98de897f65311296d00b83f4f5cb0a`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.27-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6b3f13c88059ae711cd5f74c2cbf17b098541c0277e04c22da87002af9f73d3e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116871767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1912215ebc6c9e79834773575de4b4cf7328f76096c639809f91712acf033d`
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
# Thu, 21 Jan 2021 05:42:21 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 05:42:23 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:43:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:43:09 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:43:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:43:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:43:13 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:43:14 GMT
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
	-	`sha256:30503b1b816b67d95b85a2aa5bb4629030261cdf070f519263adc4cc9b467b94`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2401763c58fae1af4f54b24fb8bcd8ef12c25a573ed6add42c69f46727f1a2ee`  
		Last Modified: Thu, 21 Jan 2021 05:48:53 GMT  
		Size: 81.7 MB (81698789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784582ef68840074e18c294150aac11cdbd3d836587d2d38dc8c81720898d265`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 4.9 KB (4915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b92b5508c1b68482631cefdc59114a74152fb7d29f11516374ae635952b322`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.27-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:70c97f38ef062d473d3502708ff31798ca03cfa1aeff6168565a8dd75bf953f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129052717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf901d1f35ca5ea3e90d5415f820d5e973b442a75aaabf6709fb89ff62b7e119`
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
# Thu, 21 Jan 2021 06:03:53 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 06:04:08 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:07:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:07:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:07:58 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:08:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:08:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:08:17 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:08:25 GMT
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
	-	`sha256:10cabac2f70a6357ef272cb67c3cefcf1faa7004bd07f4950fcfaa8039bafa7e`  
		Last Modified: Thu, 21 Jan 2021 06:28:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc0c94895146903b4e9c57d85817555cf21b36e302f7c64e2d6fb05d017b6fd`  
		Last Modified: Thu, 21 Jan 2021 06:28:54 GMT  
		Size: 86.6 MB (86567793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5feb6c8acd8c1db342471fd22b7602f0635fba23a0a37c8d8454065bd5f1f344`  
		Last Modified: Thu, 21 Jan 2021 06:28:37 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21879422024ab16fd75f7d37b8f7b39de729a78e89b16e6a33f0016d9d0b9ed1`  
		Last Modified: Thu, 21 Jan 2021 06:28:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:820ef6569f29e76e61bcf0d6005b858037b0f49afddaa7d2943a6c0de646a6d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:3f57f61689aac8c56ebe5d184622c9fa9f0359aad4d481a5f52a74d92534540e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119247331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2abc809aea2acd3c35befc0946d09b6665098615de7b8e860b5df60d67ea396e`
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
# Thu, 21 Jan 2021 11:59:23 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 11:59:24 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:59:52 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:59:52 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:59:53 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:59:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 11:59:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:59:54 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:59:54 GMT
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
	-	`sha256:60f77f5f102cf856c02897bbcc07066c00fddbf376423d3d35e870d2894c943e`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce534039c7fd41cb524120e2e9116fac33e6229ea1a9cba14c99a0fda1868ca`  
		Last Modified: Thu, 21 Jan 2021 12:04:14 GMT  
		Size: 82.6 MB (82585884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01014da6acb1ec93717bbd1643af27a01c5a129463fed08abb06c1cc62b3d100`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ffc1a63001f827f81a88e1c5b600dbce98de897f65311296d00b83f4f5cb0a`  
		Last Modified: Thu, 21 Jan 2021 12:03:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:6b3f13c88059ae711cd5f74c2cbf17b098541c0277e04c22da87002af9f73d3e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.9 MB (116871767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1912215ebc6c9e79834773575de4b4cf7328f76096c639809f91712acf033d`
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
# Thu, 21 Jan 2021 05:42:21 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 05:42:23 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:43:07 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:43:09 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:43:10 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:43:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:43:13 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:43:14 GMT
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
	-	`sha256:30503b1b816b67d95b85a2aa5bb4629030261cdf070f519263adc4cc9b467b94`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2401763c58fae1af4f54b24fb8bcd8ef12c25a573ed6add42c69f46727f1a2ee`  
		Last Modified: Thu, 21 Jan 2021 05:48:53 GMT  
		Size: 81.7 MB (81698789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784582ef68840074e18c294150aac11cdbd3d836587d2d38dc8c81720898d265`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 4.9 KB (4915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b92b5508c1b68482631cefdc59114a74152fb7d29f11516374ae635952b322`  
		Last Modified: Thu, 21 Jan 2021 05:48:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:70c97f38ef062d473d3502708ff31798ca03cfa1aeff6168565a8dd75bf953f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.1 MB (129052717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf901d1f35ca5ea3e90d5415f820d5e973b442a75aaabf6709fb89ff62b7e119`
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
# Thu, 21 Jan 2021 06:03:53 GMT
ENV MARIADB_VERSION=1:10.3.27+maria~focal
# Thu, 21 Jan 2021 06:04:08 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:07:36 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:07:55 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:07:58 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:08:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:08:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:08:17 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:08:25 GMT
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
	-	`sha256:10cabac2f70a6357ef272cb67c3cefcf1faa7004bd07f4950fcfaa8039bafa7e`  
		Last Modified: Thu, 21 Jan 2021 06:28:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc0c94895146903b4e9c57d85817555cf21b36e302f7c64e2d6fb05d017b6fd`  
		Last Modified: Thu, 21 Jan 2021 06:28:54 GMT  
		Size: 86.6 MB (86567793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5feb6c8acd8c1db342471fd22b7602f0635fba23a0a37c8d8454065bd5f1f344`  
		Last Modified: Thu, 21 Jan 2021 06:28:37 GMT  
		Size: 4.9 KB (4921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21879422024ab16fd75f7d37b8f7b39de729a78e89b16e6a33f0016d9d0b9ed1`  
		Last Modified: Thu, 21 Jan 2021 06:28:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:cdcbe6cea1d2a0276f0f6432f8964de7be5ce8eb4d9b20dea45daa4be1305911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:9d093ee9dc45aaf7f0cce8cbd6e6dc3697d49b2adabe0f0661a17e792c6a0d86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123576581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f90ac53d5cdf0c751058782d6ea11b72e08f3a07d3c158684d6250f2b4f91b7`
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
# Thu, 21 Jan 2021 11:58:49 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 11:58:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:59:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:59:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:59:15 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:59:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 11:59:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:59:16 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:59:17 GMT
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
	-	`sha256:b071b8b8af9b55ee52cbd9b622a2f92fd460e015dfbc52b940ded8978dcee481`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c898a94b9bf2a9d93c36acd25fc7543cc0cb2e24740c8b27d6b92c686ece5a0`  
		Last Modified: Thu, 21 Jan 2021 12:03:47 GMT  
		Size: 86.9 MB (86915135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d068bfba4b3d244ff37d6e9fea07f41996d053605e7bbed08a24a09afb2c37`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad03a4eeca834dbf712a7228d0de7b0821f902eee3038dc704ef503f71aa70`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c00463ac3e9e7fe22cb55b61e8eee983646bc358ad8d5c4a6c40ecec3bfe0058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121177612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b295c0f8693647b8ea0c905a040b4e63d387cded5f652cbcee5d50150e4d9def`
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
# Thu, 21 Jan 2021 05:41:23 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 05:41:25 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:42:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:42:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:42:05 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:42:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:42:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:42:09 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:42:09 GMT
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
	-	`sha256:56ac216b27906bd1ce246ac8da9ff36c73f6e593cd6d51bded9d6f4f7abfb223`  
		Last Modified: Thu, 21 Jan 2021 05:47:50 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8ae193aa63e7ddc05f9e72de172143edc986515e56904e5ac04ffaf9e1447f`  
		Last Modified: Thu, 21 Jan 2021 05:48:13 GMT  
		Size: 86.0 MB (86004634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c426ae8a1a2f014d6d23955f98981f8494b1b5467d11f6bf71c65df560979fd4`  
		Last Modified: Thu, 21 Jan 2021 05:47:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9d9bf61f0779e7d5cf4e794c5501384dca06f25d0e6dbd9fe9d93499451078`  
		Last Modified: Thu, 21 Jan 2021 05:47:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:be295a01e387f124d36598750381053450475462c1c112335c2feaeb1c74f3ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133513612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e95194fc3360791e15ba0b63228ab2ffbb23a3c99fe2dde0c8d0d09158e8e5`
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
# Thu, 21 Jan 2021 05:59:08 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 05:59:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:02:37 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:02:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:02:57 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:03:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:03:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:03:19 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:03:26 GMT
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
	-	`sha256:5c798ab766e7133f84c3fe7b26380fd4ea9d1e100793f66ad02b4c6ae8d2b965`  
		Last Modified: Thu, 21 Jan 2021 06:24:15 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0522e6feec8b5be41f793fd4dfe911a73ea0a9dd80fb455c0c4ceb7b320f5fc`  
		Last Modified: Thu, 21 Jan 2021 06:24:34 GMT  
		Size: 91.0 MB (91028692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab99bf53c3692087fc050eb59236cb79d1e5a58c8f7178aea6ff9a8e8b8861ec`  
		Last Modified: Thu, 21 Jan 2021 06:24:14 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c216ee14539042ac8a2f413b870d946e83d302f8ba24166ac4d4484f69799ec6`  
		Last Modified: Thu, 21 Jan 2021 06:24:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.17`

```console
$ docker pull mariadb@sha256:cdcbe6cea1d2a0276f0f6432f8964de7be5ce8eb4d9b20dea45daa4be1305911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.17` - linux; amd64

```console
$ docker pull mariadb@sha256:9d093ee9dc45aaf7f0cce8cbd6e6dc3697d49b2adabe0f0661a17e792c6a0d86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123576581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f90ac53d5cdf0c751058782d6ea11b72e08f3a07d3c158684d6250f2b4f91b7`
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
# Thu, 21 Jan 2021 11:58:49 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 11:58:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:59:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:59:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:59:15 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:59:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 11:59:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:59:16 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:59:17 GMT
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
	-	`sha256:b071b8b8af9b55ee52cbd9b622a2f92fd460e015dfbc52b940ded8978dcee481`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c898a94b9bf2a9d93c36acd25fc7543cc0cb2e24740c8b27d6b92c686ece5a0`  
		Last Modified: Thu, 21 Jan 2021 12:03:47 GMT  
		Size: 86.9 MB (86915135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d068bfba4b3d244ff37d6e9fea07f41996d053605e7bbed08a24a09afb2c37`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad03a4eeca834dbf712a7228d0de7b0821f902eee3038dc704ef503f71aa70`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.17` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c00463ac3e9e7fe22cb55b61e8eee983646bc358ad8d5c4a6c40ecec3bfe0058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121177612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b295c0f8693647b8ea0c905a040b4e63d387cded5f652cbcee5d50150e4d9def`
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
# Thu, 21 Jan 2021 05:41:23 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 05:41:25 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:42:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:42:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:42:05 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:42:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:42:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:42:09 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:42:09 GMT
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
	-	`sha256:56ac216b27906bd1ce246ac8da9ff36c73f6e593cd6d51bded9d6f4f7abfb223`  
		Last Modified: Thu, 21 Jan 2021 05:47:50 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8ae193aa63e7ddc05f9e72de172143edc986515e56904e5ac04ffaf9e1447f`  
		Last Modified: Thu, 21 Jan 2021 05:48:13 GMT  
		Size: 86.0 MB (86004634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c426ae8a1a2f014d6d23955f98981f8494b1b5467d11f6bf71c65df560979fd4`  
		Last Modified: Thu, 21 Jan 2021 05:47:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9d9bf61f0779e7d5cf4e794c5501384dca06f25d0e6dbd9fe9d93499451078`  
		Last Modified: Thu, 21 Jan 2021 05:47:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.17` - linux; ppc64le

```console
$ docker pull mariadb@sha256:be295a01e387f124d36598750381053450475462c1c112335c2feaeb1c74f3ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133513612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e95194fc3360791e15ba0b63228ab2ffbb23a3c99fe2dde0c8d0d09158e8e5`
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
# Thu, 21 Jan 2021 05:59:08 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 05:59:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:02:37 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:02:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:02:57 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:03:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:03:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:03:19 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:03:26 GMT
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
	-	`sha256:5c798ab766e7133f84c3fe7b26380fd4ea9d1e100793f66ad02b4c6ae8d2b965`  
		Last Modified: Thu, 21 Jan 2021 06:24:15 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0522e6feec8b5be41f793fd4dfe911a73ea0a9dd80fb455c0c4ceb7b320f5fc`  
		Last Modified: Thu, 21 Jan 2021 06:24:34 GMT  
		Size: 91.0 MB (91028692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab99bf53c3692087fc050eb59236cb79d1e5a58c8f7178aea6ff9a8e8b8861ec`  
		Last Modified: Thu, 21 Jan 2021 06:24:14 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c216ee14539042ac8a2f413b870d946e83d302f8ba24166ac4d4484f69799ec6`  
		Last Modified: Thu, 21 Jan 2021 06:24:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.17-focal`

```console
$ docker pull mariadb@sha256:cdcbe6cea1d2a0276f0f6432f8964de7be5ce8eb4d9b20dea45daa4be1305911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.17-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9d093ee9dc45aaf7f0cce8cbd6e6dc3697d49b2adabe0f0661a17e792c6a0d86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123576581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f90ac53d5cdf0c751058782d6ea11b72e08f3a07d3c158684d6250f2b4f91b7`
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
# Thu, 21 Jan 2021 11:58:49 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 11:58:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:59:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:59:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:59:15 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:59:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 11:59:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:59:16 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:59:17 GMT
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
	-	`sha256:b071b8b8af9b55ee52cbd9b622a2f92fd460e015dfbc52b940ded8978dcee481`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c898a94b9bf2a9d93c36acd25fc7543cc0cb2e24740c8b27d6b92c686ece5a0`  
		Last Modified: Thu, 21 Jan 2021 12:03:47 GMT  
		Size: 86.9 MB (86915135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d068bfba4b3d244ff37d6e9fea07f41996d053605e7bbed08a24a09afb2c37`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad03a4eeca834dbf712a7228d0de7b0821f902eee3038dc704ef503f71aa70`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.17-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c00463ac3e9e7fe22cb55b61e8eee983646bc358ad8d5c4a6c40ecec3bfe0058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121177612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b295c0f8693647b8ea0c905a040b4e63d387cded5f652cbcee5d50150e4d9def`
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
# Thu, 21 Jan 2021 05:41:23 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 05:41:25 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:42:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:42:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:42:05 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:42:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:42:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:42:09 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:42:09 GMT
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
	-	`sha256:56ac216b27906bd1ce246ac8da9ff36c73f6e593cd6d51bded9d6f4f7abfb223`  
		Last Modified: Thu, 21 Jan 2021 05:47:50 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8ae193aa63e7ddc05f9e72de172143edc986515e56904e5ac04ffaf9e1447f`  
		Last Modified: Thu, 21 Jan 2021 05:48:13 GMT  
		Size: 86.0 MB (86004634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c426ae8a1a2f014d6d23955f98981f8494b1b5467d11f6bf71c65df560979fd4`  
		Last Modified: Thu, 21 Jan 2021 05:47:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9d9bf61f0779e7d5cf4e794c5501384dca06f25d0e6dbd9fe9d93499451078`  
		Last Modified: Thu, 21 Jan 2021 05:47:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.17-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:be295a01e387f124d36598750381053450475462c1c112335c2feaeb1c74f3ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133513612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e95194fc3360791e15ba0b63228ab2ffbb23a3c99fe2dde0c8d0d09158e8e5`
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
# Thu, 21 Jan 2021 05:59:08 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 05:59:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:02:37 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:02:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:02:57 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:03:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:03:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:03:19 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:03:26 GMT
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
	-	`sha256:5c798ab766e7133f84c3fe7b26380fd4ea9d1e100793f66ad02b4c6ae8d2b965`  
		Last Modified: Thu, 21 Jan 2021 06:24:15 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0522e6feec8b5be41f793fd4dfe911a73ea0a9dd80fb455c0c4ceb7b320f5fc`  
		Last Modified: Thu, 21 Jan 2021 06:24:34 GMT  
		Size: 91.0 MB (91028692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab99bf53c3692087fc050eb59236cb79d1e5a58c8f7178aea6ff9a8e8b8861ec`  
		Last Modified: Thu, 21 Jan 2021 06:24:14 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c216ee14539042ac8a2f413b870d946e83d302f8ba24166ac4d4484f69799ec6`  
		Last Modified: Thu, 21 Jan 2021 06:24:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:cdcbe6cea1d2a0276f0f6432f8964de7be5ce8eb4d9b20dea45daa4be1305911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:9d093ee9dc45aaf7f0cce8cbd6e6dc3697d49b2adabe0f0661a17e792c6a0d86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 MB (123576581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f90ac53d5cdf0c751058782d6ea11b72e08f3a07d3c158684d6250f2b4f91b7`
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
# Thu, 21 Jan 2021 11:58:49 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 11:58:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:59:15 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:59:15 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:59:15 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:59:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 11:59:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:59:16 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:59:17 GMT
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
	-	`sha256:b071b8b8af9b55ee52cbd9b622a2f92fd460e015dfbc52b940ded8978dcee481`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c898a94b9bf2a9d93c36acd25fc7543cc0cb2e24740c8b27d6b92c686ece5a0`  
		Last Modified: Thu, 21 Jan 2021 12:03:47 GMT  
		Size: 86.9 MB (86915135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d068bfba4b3d244ff37d6e9fea07f41996d053605e7bbed08a24a09afb2c37`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad03a4eeca834dbf712a7228d0de7b0821f902eee3038dc704ef503f71aa70`  
		Last Modified: Thu, 21 Jan 2021 12:03:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c00463ac3e9e7fe22cb55b61e8eee983646bc358ad8d5c4a6c40ecec3bfe0058
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121177612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b295c0f8693647b8ea0c905a040b4e63d387cded5f652cbcee5d50150e4d9def`
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
# Thu, 21 Jan 2021 05:41:23 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 05:41:25 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:42:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:42:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:42:05 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:42:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 05:42:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:42:09 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:42:09 GMT
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
	-	`sha256:56ac216b27906bd1ce246ac8da9ff36c73f6e593cd6d51bded9d6f4f7abfb223`  
		Last Modified: Thu, 21 Jan 2021 05:47:50 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8ae193aa63e7ddc05f9e72de172143edc986515e56904e5ac04ffaf9e1447f`  
		Last Modified: Thu, 21 Jan 2021 05:48:13 GMT  
		Size: 86.0 MB (86004634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c426ae8a1a2f014d6d23955f98981f8494b1b5467d11f6bf71c65df560979fd4`  
		Last Modified: Thu, 21 Jan 2021 05:47:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9d9bf61f0779e7d5cf4e794c5501384dca06f25d0e6dbd9fe9d93499451078`  
		Last Modified: Thu, 21 Jan 2021 05:47:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:be295a01e387f124d36598750381053450475462c1c112335c2feaeb1c74f3ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133513612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e95194fc3360791e15ba0b63228ab2ffbb23a3c99fe2dde0c8d0d09158e8e5`
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
# Thu, 21 Jan 2021 05:59:08 GMT
ENV MARIADB_VERSION=1:10.4.17+maria~focal
# Thu, 21 Jan 2021 05:59:16 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 06:02:37 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 06:02:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 06:02:57 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 06:03:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Jan 2021 06:03:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 06:03:19 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 06:03:26 GMT
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
	-	`sha256:5c798ab766e7133f84c3fe7b26380fd4ea9d1e100793f66ad02b4c6ae8d2b965`  
		Last Modified: Thu, 21 Jan 2021 06:24:15 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0522e6feec8b5be41f793fd4dfe911a73ea0a9dd80fb455c0c4ceb7b320f5fc`  
		Last Modified: Thu, 21 Jan 2021 06:24:34 GMT  
		Size: 91.0 MB (91028692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab99bf53c3692087fc050eb59236cb79d1e5a58c8f7178aea6ff9a8e8b8861ec`  
		Last Modified: Thu, 21 Jan 2021 06:24:14 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c216ee14539042ac8a2f413b870d946e83d302f8ba24166ac4d4484f69799ec6`  
		Last Modified: Thu, 21 Jan 2021 06:24:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:8040983db146f729749081c6b216a19d52e0973134e2e34c0b4fd87f48bc15b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:03fb19fa5729856ec8c8ed23d421ed1ab6c0e2d63fdf2b1bd8d311025e228a9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125593666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade39f0469a3fa0e5f907e4dd7861a4e77573b0757bd4055a7b4c52baea58590`
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
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 11:58:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:58:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:58:39 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:58:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:58:39 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:58:39 GMT
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
	-	`sha256:5d1a793b093fb66b368496d9fc031d57477617a83485edd703c254af153a8e92`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477cd2b3eba82e02507024ebdc4dee18f00503fca5308d5d4258dc1a2fd29741`  
		Last Modified: Thu, 21 Jan 2021 12:03:06 GMT  
		Size: 88.9 MB (88932340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40245454316697c87c982e323046c544d7838a1758bf9f85b8fdc0de8e8cf4c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c892a2d0194f19d0aa29fa165cdbfeb6be619cbf68b7a9f715369f7f08c05311
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123207507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3ab601101c5c8e7e2238bb43637af4113de1d73fea960e84f06a91663ad364`
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
# Thu, 21 Jan 2021 05:40:28 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:40:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:41:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:41:05 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:41:06 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:41:07 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:41:08 GMT
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
	-	`sha256:01b09912c33f2e7b6a76320f2c201590899ee9b65c0a74c459e877702bbed84f`  
		Last Modified: Thu, 21 Jan 2021 05:47:04 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bd2c4c297c8d6742d93d7dcd7fa909f85e44eb27209214b362fc52f48a1d48`  
		Last Modified: Thu, 21 Jan 2021 05:47:29 GMT  
		Size: 88.0 MB (88034645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c6e38659e4a0759fb2b50eb8fa140f50e1abdc8038bb5cb07209c908d80fca`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:998603c1d9d5ce3c30340897c9071dfaac88b3b8bedf1c351d207dfdad99a401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135593595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd15ad097e80bfded8f3563be92ffefc5e426a4f65a5b3b4d3ea04f6c44c07a`
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
# Thu, 21 Jan 2021 05:54:46 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:54:58 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:58:16 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:58:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:58:31 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:58:40 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:58:44 GMT
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
	-	`sha256:d17dc5940401537ceb8f16e75f7b3e24ed0227778aa65a34487ed355ec81b5a8`  
		Last Modified: Thu, 21 Jan 2021 06:23:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6539b7b968359217718b2cfdc33635f618728f4db73eff20f977cc203783b`  
		Last Modified: Thu, 21 Jan 2021 06:23:42 GMT  
		Size: 93.1 MB (93108795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412f01454a1c306983d7b46c8dca3ae6d371cd540b7d3be8cf70d8b891f8b432`  
		Last Modified: Thu, 21 Jan 2021 06:23:18 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.8`

```console
$ docker pull mariadb@sha256:8040983db146f729749081c6b216a19d52e0973134e2e34c0b4fd87f48bc15b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.8` - linux; amd64

```console
$ docker pull mariadb@sha256:03fb19fa5729856ec8c8ed23d421ed1ab6c0e2d63fdf2b1bd8d311025e228a9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125593666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade39f0469a3fa0e5f907e4dd7861a4e77573b0757bd4055a7b4c52baea58590`
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
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 11:58:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:58:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:58:39 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:58:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:58:39 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:58:39 GMT
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
	-	`sha256:5d1a793b093fb66b368496d9fc031d57477617a83485edd703c254af153a8e92`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477cd2b3eba82e02507024ebdc4dee18f00503fca5308d5d4258dc1a2fd29741`  
		Last Modified: Thu, 21 Jan 2021 12:03:06 GMT  
		Size: 88.9 MB (88932340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40245454316697c87c982e323046c544d7838a1758bf9f85b8fdc0de8e8cf4c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.8` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c892a2d0194f19d0aa29fa165cdbfeb6be619cbf68b7a9f715369f7f08c05311
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123207507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3ab601101c5c8e7e2238bb43637af4113de1d73fea960e84f06a91663ad364`
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
# Thu, 21 Jan 2021 05:40:28 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:40:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:41:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:41:05 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:41:06 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:41:07 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:41:08 GMT
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
	-	`sha256:01b09912c33f2e7b6a76320f2c201590899ee9b65c0a74c459e877702bbed84f`  
		Last Modified: Thu, 21 Jan 2021 05:47:04 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bd2c4c297c8d6742d93d7dcd7fa909f85e44eb27209214b362fc52f48a1d48`  
		Last Modified: Thu, 21 Jan 2021 05:47:29 GMT  
		Size: 88.0 MB (88034645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c6e38659e4a0759fb2b50eb8fa140f50e1abdc8038bb5cb07209c908d80fca`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.8` - linux; ppc64le

```console
$ docker pull mariadb@sha256:998603c1d9d5ce3c30340897c9071dfaac88b3b8bedf1c351d207dfdad99a401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135593595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd15ad097e80bfded8f3563be92ffefc5e426a4f65a5b3b4d3ea04f6c44c07a`
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
# Thu, 21 Jan 2021 05:54:46 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:54:58 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:58:16 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:58:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:58:31 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:58:40 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:58:44 GMT
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
	-	`sha256:d17dc5940401537ceb8f16e75f7b3e24ed0227778aa65a34487ed355ec81b5a8`  
		Last Modified: Thu, 21 Jan 2021 06:23:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6539b7b968359217718b2cfdc33635f618728f4db73eff20f977cc203783b`  
		Last Modified: Thu, 21 Jan 2021 06:23:42 GMT  
		Size: 93.1 MB (93108795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412f01454a1c306983d7b46c8dca3ae6d371cd540b7d3be8cf70d8b891f8b432`  
		Last Modified: Thu, 21 Jan 2021 06:23:18 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.8-focal`

```console
$ docker pull mariadb@sha256:8040983db146f729749081c6b216a19d52e0973134e2e34c0b4fd87f48bc15b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.8-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:03fb19fa5729856ec8c8ed23d421ed1ab6c0e2d63fdf2b1bd8d311025e228a9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125593666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade39f0469a3fa0e5f907e4dd7861a4e77573b0757bd4055a7b4c52baea58590`
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
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 11:58:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:58:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:58:39 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:58:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:58:39 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:58:39 GMT
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
	-	`sha256:5d1a793b093fb66b368496d9fc031d57477617a83485edd703c254af153a8e92`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477cd2b3eba82e02507024ebdc4dee18f00503fca5308d5d4258dc1a2fd29741`  
		Last Modified: Thu, 21 Jan 2021 12:03:06 GMT  
		Size: 88.9 MB (88932340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40245454316697c87c982e323046c544d7838a1758bf9f85b8fdc0de8e8cf4c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.8-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c892a2d0194f19d0aa29fa165cdbfeb6be619cbf68b7a9f715369f7f08c05311
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123207507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3ab601101c5c8e7e2238bb43637af4113de1d73fea960e84f06a91663ad364`
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
# Thu, 21 Jan 2021 05:40:28 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:40:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:41:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:41:05 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:41:06 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:41:07 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:41:08 GMT
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
	-	`sha256:01b09912c33f2e7b6a76320f2c201590899ee9b65c0a74c459e877702bbed84f`  
		Last Modified: Thu, 21 Jan 2021 05:47:04 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bd2c4c297c8d6742d93d7dcd7fa909f85e44eb27209214b362fc52f48a1d48`  
		Last Modified: Thu, 21 Jan 2021 05:47:29 GMT  
		Size: 88.0 MB (88034645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c6e38659e4a0759fb2b50eb8fa140f50e1abdc8038bb5cb07209c908d80fca`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.8-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:998603c1d9d5ce3c30340897c9071dfaac88b3b8bedf1c351d207dfdad99a401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135593595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd15ad097e80bfded8f3563be92ffefc5e426a4f65a5b3b4d3ea04f6c44c07a`
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
# Thu, 21 Jan 2021 05:54:46 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:54:58 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:58:16 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:58:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:58:31 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:58:40 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:58:44 GMT
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
	-	`sha256:d17dc5940401537ceb8f16e75f7b3e24ed0227778aa65a34487ed355ec81b5a8`  
		Last Modified: Thu, 21 Jan 2021 06:23:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6539b7b968359217718b2cfdc33635f618728f4db73eff20f977cc203783b`  
		Last Modified: Thu, 21 Jan 2021 06:23:42 GMT  
		Size: 93.1 MB (93108795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412f01454a1c306983d7b46c8dca3ae6d371cd540b7d3be8cf70d8b891f8b432`  
		Last Modified: Thu, 21 Jan 2021 06:23:18 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:8040983db146f729749081c6b216a19d52e0973134e2e34c0b4fd87f48bc15b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:03fb19fa5729856ec8c8ed23d421ed1ab6c0e2d63fdf2b1bd8d311025e228a9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125593666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade39f0469a3fa0e5f907e4dd7861a4e77573b0757bd4055a7b4c52baea58590`
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
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 11:58:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:58:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:58:39 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:58:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:58:39 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:58:39 GMT
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
	-	`sha256:5d1a793b093fb66b368496d9fc031d57477617a83485edd703c254af153a8e92`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477cd2b3eba82e02507024ebdc4dee18f00503fca5308d5d4258dc1a2fd29741`  
		Last Modified: Thu, 21 Jan 2021 12:03:06 GMT  
		Size: 88.9 MB (88932340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40245454316697c87c982e323046c544d7838a1758bf9f85b8fdc0de8e8cf4c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c892a2d0194f19d0aa29fa165cdbfeb6be619cbf68b7a9f715369f7f08c05311
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123207507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3ab601101c5c8e7e2238bb43637af4113de1d73fea960e84f06a91663ad364`
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
# Thu, 21 Jan 2021 05:40:28 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:40:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:41:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:41:05 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:41:06 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:41:07 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:41:08 GMT
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
	-	`sha256:01b09912c33f2e7b6a76320f2c201590899ee9b65c0a74c459e877702bbed84f`  
		Last Modified: Thu, 21 Jan 2021 05:47:04 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bd2c4c297c8d6742d93d7dcd7fa909f85e44eb27209214b362fc52f48a1d48`  
		Last Modified: Thu, 21 Jan 2021 05:47:29 GMT  
		Size: 88.0 MB (88034645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c6e38659e4a0759fb2b50eb8fa140f50e1abdc8038bb5cb07209c908d80fca`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:998603c1d9d5ce3c30340897c9071dfaac88b3b8bedf1c351d207dfdad99a401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135593595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd15ad097e80bfded8f3563be92ffefc5e426a4f65a5b3b4d3ea04f6c44c07a`
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
# Thu, 21 Jan 2021 05:54:46 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:54:58 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:58:16 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:58:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:58:31 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:58:40 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:58:44 GMT
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
	-	`sha256:d17dc5940401537ceb8f16e75f7b3e24ed0227778aa65a34487ed355ec81b5a8`  
		Last Modified: Thu, 21 Jan 2021 06:23:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6539b7b968359217718b2cfdc33635f618728f4db73eff20f977cc203783b`  
		Last Modified: Thu, 21 Jan 2021 06:23:42 GMT  
		Size: 93.1 MB (93108795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412f01454a1c306983d7b46c8dca3ae6d371cd540b7d3be8cf70d8b891f8b432`  
		Last Modified: Thu, 21 Jan 2021 06:23:18 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:8040983db146f729749081c6b216a19d52e0973134e2e34c0b4fd87f48bc15b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:03fb19fa5729856ec8c8ed23d421ed1ab6c0e2d63fdf2b1bd8d311025e228a9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125593666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade39f0469a3fa0e5f907e4dd7861a4e77573b0757bd4055a7b4c52baea58590`
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
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 11:58:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:58:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:58:39 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:58:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:58:39 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:58:39 GMT
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
	-	`sha256:5d1a793b093fb66b368496d9fc031d57477617a83485edd703c254af153a8e92`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477cd2b3eba82e02507024ebdc4dee18f00503fca5308d5d4258dc1a2fd29741`  
		Last Modified: Thu, 21 Jan 2021 12:03:06 GMT  
		Size: 88.9 MB (88932340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40245454316697c87c982e323046c544d7838a1758bf9f85b8fdc0de8e8cf4c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c892a2d0194f19d0aa29fa165cdbfeb6be619cbf68b7a9f715369f7f08c05311
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123207507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3ab601101c5c8e7e2238bb43637af4113de1d73fea960e84f06a91663ad364`
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
# Thu, 21 Jan 2021 05:40:28 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:40:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:41:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:41:05 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:41:06 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:41:07 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:41:08 GMT
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
	-	`sha256:01b09912c33f2e7b6a76320f2c201590899ee9b65c0a74c459e877702bbed84f`  
		Last Modified: Thu, 21 Jan 2021 05:47:04 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bd2c4c297c8d6742d93d7dcd7fa909f85e44eb27209214b362fc52f48a1d48`  
		Last Modified: Thu, 21 Jan 2021 05:47:29 GMT  
		Size: 88.0 MB (88034645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c6e38659e4a0759fb2b50eb8fa140f50e1abdc8038bb5cb07209c908d80fca`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:998603c1d9d5ce3c30340897c9071dfaac88b3b8bedf1c351d207dfdad99a401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135593595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd15ad097e80bfded8f3563be92ffefc5e426a4f65a5b3b4d3ea04f6c44c07a`
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
# Thu, 21 Jan 2021 05:54:46 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:54:58 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:58:16 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:58:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:58:31 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:58:40 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:58:44 GMT
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
	-	`sha256:d17dc5940401537ceb8f16e75f7b3e24ed0227778aa65a34487ed355ec81b5a8`  
		Last Modified: Thu, 21 Jan 2021 06:23:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6539b7b968359217718b2cfdc33635f618728f4db73eff20f977cc203783b`  
		Last Modified: Thu, 21 Jan 2021 06:23:42 GMT  
		Size: 93.1 MB (93108795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412f01454a1c306983d7b46c8dca3ae6d371cd540b7d3be8cf70d8b891f8b432`  
		Last Modified: Thu, 21 Jan 2021 06:23:18 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:8040983db146f729749081c6b216a19d52e0973134e2e34c0b4fd87f48bc15b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:03fb19fa5729856ec8c8ed23d421ed1ab6c0e2d63fdf2b1bd8d311025e228a9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125593666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade39f0469a3fa0e5f907e4dd7861a4e77573b0757bd4055a7b4c52baea58590`
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
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 11:58:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:58:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:58:39 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:58:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:58:39 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:58:39 GMT
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
	-	`sha256:5d1a793b093fb66b368496d9fc031d57477617a83485edd703c254af153a8e92`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477cd2b3eba82e02507024ebdc4dee18f00503fca5308d5d4258dc1a2fd29741`  
		Last Modified: Thu, 21 Jan 2021 12:03:06 GMT  
		Size: 88.9 MB (88932340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40245454316697c87c982e323046c544d7838a1758bf9f85b8fdc0de8e8cf4c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c892a2d0194f19d0aa29fa165cdbfeb6be619cbf68b7a9f715369f7f08c05311
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123207507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3ab601101c5c8e7e2238bb43637af4113de1d73fea960e84f06a91663ad364`
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
# Thu, 21 Jan 2021 05:40:28 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:40:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:41:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:41:05 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:41:06 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:41:07 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:41:08 GMT
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
	-	`sha256:01b09912c33f2e7b6a76320f2c201590899ee9b65c0a74c459e877702bbed84f`  
		Last Modified: Thu, 21 Jan 2021 05:47:04 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bd2c4c297c8d6742d93d7dcd7fa909f85e44eb27209214b362fc52f48a1d48`  
		Last Modified: Thu, 21 Jan 2021 05:47:29 GMT  
		Size: 88.0 MB (88034645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c6e38659e4a0759fb2b50eb8fa140f50e1abdc8038bb5cb07209c908d80fca`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:998603c1d9d5ce3c30340897c9071dfaac88b3b8bedf1c351d207dfdad99a401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135593595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd15ad097e80bfded8f3563be92ffefc5e426a4f65a5b3b4d3ea04f6c44c07a`
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
# Thu, 21 Jan 2021 05:54:46 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:54:58 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:58:16 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:58:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:58:31 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:58:40 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:58:44 GMT
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
	-	`sha256:d17dc5940401537ceb8f16e75f7b3e24ed0227778aa65a34487ed355ec81b5a8`  
		Last Modified: Thu, 21 Jan 2021 06:23:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6539b7b968359217718b2cfdc33635f618728f4db73eff20f977cc203783b`  
		Last Modified: Thu, 21 Jan 2021 06:23:42 GMT  
		Size: 93.1 MB (93108795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412f01454a1c306983d7b46c8dca3ae6d371cd540b7d3be8cf70d8b891f8b432`  
		Last Modified: Thu, 21 Jan 2021 06:23:18 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:8040983db146f729749081c6b216a19d52e0973134e2e34c0b4fd87f48bc15b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:03fb19fa5729856ec8c8ed23d421ed1ab6c0e2d63fdf2b1bd8d311025e228a9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125593666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade39f0469a3fa0e5f907e4dd7861a4e77573b0757bd4055a7b4c52baea58590`
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
# Thu, 21 Jan 2021 11:58:09 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 11:58:10 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 11:58:38 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 11:58:39 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 11:58:39 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 11:58:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 11:58:39 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 11:58:39 GMT
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
	-	`sha256:5d1a793b093fb66b368496d9fc031d57477617a83485edd703c254af153a8e92`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477cd2b3eba82e02507024ebdc4dee18f00503fca5308d5d4258dc1a2fd29741`  
		Last Modified: Thu, 21 Jan 2021 12:03:06 GMT  
		Size: 88.9 MB (88932340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40245454316697c87c982e323046c544d7838a1758bf9f85b8fdc0de8e8cf4c9`  
		Last Modified: Thu, 21 Jan 2021 12:02:50 GMT  
		Size: 4.9 KB (4918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:c892a2d0194f19d0aa29fa165cdbfeb6be619cbf68b7a9f715369f7f08c05311
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123207507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3ab601101c5c8e7e2238bb43637af4113de1d73fea960e84f06a91663ad364`
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
# Thu, 21 Jan 2021 05:40:28 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:40:29 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:41:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:41:05 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:41:06 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:41:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:41:07 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:41:08 GMT
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
	-	`sha256:01b09912c33f2e7b6a76320f2c201590899ee9b65c0a74c459e877702bbed84f`  
		Last Modified: Thu, 21 Jan 2021 05:47:04 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bd2c4c297c8d6742d93d7dcd7fa909f85e44eb27209214b362fc52f48a1d48`  
		Last Modified: Thu, 21 Jan 2021 05:47:29 GMT  
		Size: 88.0 MB (88034645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c6e38659e4a0759fb2b50eb8fa140f50e1abdc8038bb5cb07209c908d80fca`  
		Last Modified: Thu, 21 Jan 2021 05:47:05 GMT  
		Size: 4.9 KB (4919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:998603c1d9d5ce3c30340897c9071dfaac88b3b8bedf1c351d207dfdad99a401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135593595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd15ad097e80bfded8f3563be92ffefc5e426a4f65a5b3b4d3ea04f6c44c07a`
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
# Thu, 21 Jan 2021 05:54:46 GMT
ENV MARIADB_VERSION=1:10.5.8+maria~focal
# Thu, 21 Jan 2021 05:54:58 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 21 Jan 2021 05:58:16 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 21 Jan 2021 05:58:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 21 Jan 2021 05:58:31 GMT
COPY file:ea9c4b6befdd0eb133ee54ae54d4237bcd96ac6ceb915a1044533c52e382ec53 in /usr/local/bin/ 
# Thu, 21 Jan 2021 05:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:58:40 GMT
EXPOSE 3306
# Thu, 21 Jan 2021 05:58:44 GMT
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
	-	`sha256:d17dc5940401537ceb8f16e75f7b3e24ed0227778aa65a34487ed355ec81b5a8`  
		Last Modified: Thu, 21 Jan 2021 06:23:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6539b7b968359217718b2cfdc33635f618728f4db73eff20f977cc203783b`  
		Last Modified: Thu, 21 Jan 2021 06:23:42 GMT  
		Size: 93.1 MB (93108795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412f01454a1c306983d7b46c8dca3ae6d371cd540b7d3be8cf70d8b891f8b432`  
		Last Modified: Thu, 21 Jan 2021 06:23:18 GMT  
		Size: 4.9 KB (4917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
