<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mariadb`

-	[`mariadb:10`](#mariadb10)
-	[`mariadb:10.1`](#mariadb101)
-	[`mariadb:10.1.46`](#mariadb10146)
-	[`mariadb:10.1.46-bionic`](#mariadb10146-bionic)
-	[`mariadb:10.1-bionic`](#mariadb101-bionic)
-	[`mariadb:10.2`](#mariadb102)
-	[`mariadb:10.2.33`](#mariadb10233)
-	[`mariadb:10.2.33-bionic`](#mariadb10233-bionic)
-	[`mariadb:10.2-bionic`](#mariadb102-bionic)
-	[`mariadb:10.3`](#mariadb103)
-	[`mariadb:10.3.24`](#mariadb10324)
-	[`mariadb:10.3.24-focal`](#mariadb10324-focal)
-	[`mariadb:10.3-focal`](#mariadb103-focal)
-	[`mariadb:10.4`](#mariadb104)
-	[`mariadb:10.4.14`](#mariadb10414)
-	[`mariadb:10.4.14-focal`](#mariadb10414-focal)
-	[`mariadb:10.4-focal`](#mariadb104-focal)
-	[`mariadb:10.5`](#mariadb105)
-	[`mariadb:10.5.5`](#mariadb1055)
-	[`mariadb:10.5.5-focal`](#mariadb1055-focal)
-	[`mariadb:10.5-focal`](#mariadb105-focal)
-	[`mariadb:10-focal`](#mariadb10-focal)
-	[`mariadb:focal`](#mariadbfocal)
-	[`mariadb:latest`](#mariadblatest)

## `mariadb:10`

```console
$ docker pull mariadb@sha256:d4138c98d16f605afc697e04e7acc9da49c455441a5f6fc85ac97e758eddc6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10` - linux; amd64

```console
$ docker pull mariadb@sha256:49c69c49cd3a725dba2e2687efc573160b16ec841c00c8a14858833050538bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125548061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff8572fa8c9edd0d2f88f03f4dc6d0e6e0c6b03be8e97bae4efd8ba76f45f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 01:08:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:09:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:09:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:09:26 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:09:27 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:09:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0222c6c4a45266f80f02da181a859e16c1746abe2cd1efda692ee4c9fa8a92a5`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab34d00af2f2502f1a8fd16103bf01ac430298666bfdfea989d8a2ac5193cf6`  
		Last Modified: Thu, 17 Sep 2020 01:13:45 GMT  
		Size: 88.9 MB (88902202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb48a5d6fdc6e4e1d8b91b2f30d10947db49be0ce584162fdead9de45bd909ba`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ffb01b700175307f942c997707101d39b938faf6b93ce97fbf17cbb7a0b06d66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123199206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89c7551a9f203b5bee56c2843a7ea98e5c34f6c5a8fab93cab697e5d55d04d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:31:43 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 00:31:44 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 00:31:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:32:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:32:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:32:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:32:26 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:32:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a96525514d40a4b5fa80950555be20f4aacb9a9271898d6ccccea5249badb`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fadbb2548d657860f32dc7d8c389fed772825c82c0d1d3b8bd7a376dbf414e`  
		Last Modified: Thu, 17 Sep 2020 00:38:35 GMT  
		Size: 88.0 MB (88047764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b2f72fd388ebb0795799efcfaff3b3c81b5e91e5fbde3cb56c24e9162efc2`  
		Last Modified: Thu, 17 Sep 2020 00:38:09 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8e30af10e119a02913a96b7d011c49f4c8e0bf868b93abae93b42c0f7a9c92ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135633547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b12d26459ccb7e6a7cbd83d66d721c98a144f18f44f189b21cc3993df05caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:05:24 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 19 Aug 2020 23:05:31 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Wed, 19 Aug 2020 23:05:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:12:01 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:12:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:12:12 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:12:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:12:18 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:12:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3de7a14dd93d9c85fd1768b2474e3bac42e73a9413a78be18d119cd2b3699d`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cebafb1fc8f371df5ff85fe7ed5667891f1c279eb78fdf0ff64635b9e53d36`  
		Last Modified: Wed, 19 Aug 2020 23:48:45 GMT  
		Size: 93.1 MB (93125609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88dba223ea3336bf9cbf0ca0c208c5e98a71b6eba6046ba8adad48a3168a7b3`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 5.1 KB (5060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1`

```console
$ docker pull mariadb@sha256:6a7a45fa10c744a1fb821752709c406eed8f052a1a8b9ffec3ae3b78dfd5e619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1` - linux; amd64

```console
$ docker pull mariadb@sha256:7712c5934462abd07b99753aeaad1b9d8db2332dc7da4264f292eebdadea9704
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113148337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:527f5e309b3de1640a11b17eea4366e2022f1b061fb85852621526d41922ab07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:11:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:11:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:11:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:11:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:11:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:32 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:11:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:12:20 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 17 Sep 2020 01:12:21 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Thu, 17 Sep 2020 01:12:21 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:13:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:13:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:13:06 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:13:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:13:07 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:13:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f302da1b612e8ea54850ec0495a374591b0a29677b6865b818490e1719d9fb`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8bf7c35412b355aaca3905c5d7ef2fd4800259be8ab1d2e7d7efa10857fedf`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 4.8 MB (4808571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324bc11a79a13859b04f667c46398832e8999729d311baed91fafc4008a4a52`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 1.3 MB (1326776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18579ec799327186b20c4ef266da0a3525f64343fefb0ea42b83568c1105c9c4`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de698a84499ad8d094edc88ede9c98efc6034c0f3dcd912916dd1d70a83f8dc6`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 930.0 KB (929998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ca9a2454258f016d19ebae1002aebd8e37b9d4dcc6a0bae0297143cf38910`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb349b72e6610d8d0078ef1077cfbbabb1857b96c7e39de299f3aa190e56915`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c42bb71bd12576c002e2043e5f87da3fa85d0cfa50fef11b19c854986b4f55`  
		Last Modified: Thu, 17 Sep 2020 01:15:13 GMT  
		Size: 79.4 MB (79369702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977bf6f7448ac99df7ce703fdfe6330842b49a2ab641f8332cf9b01475944fd`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a964f64afb85588c9daed5f65a65a9497d1a02e508241777c4b11fc2620623b`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:71266690948f44780ba1f3e9c48ca82c8f0f034c96c0b5bcb2d837d6a9b7f6bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105784494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9136f012257112f7d85a74fa68bf8a555980ad4ae3d12925df88b2a6c2e3cb8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:37 GMT
ADD file:9eedc88c2028d53a81210b52c98121dddea7e30ecfbd4d11d2a1b2bdc94a0102 in / 
# Wed, 16 Sep 2020 23:16:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:16:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:16:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:16:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:34:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:35:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:35:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:35:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:35:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:35:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:36:48 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 17 Sep 2020 00:36:48 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Thu, 17 Sep 2020 00:36:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:37:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:37:42 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:37:43 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:37:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:37:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:37:46 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:37:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2d8ee3976bc7c15c8a5279cdf0249b7e41b2a489771330d0f7affb26dd7acfb`  
		Last Modified: Fri, 04 Sep 2020 00:25:25 GMT  
		Size: 23.7 MB (23722305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007857f7b9b52d6efdfea9e086e6eaf35519130ff97bfe89970353f0ae53f13`  
		Last Modified: Wed, 16 Sep 2020 23:18:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43927e60f12d8b877ded6af5048b2ac5753fe78caba77a6bbbece4f98559b672`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d2e1ff6404f50b7e1c8366fc1c273c5b42cd576f7383176c3e65264aeebf5a`  
		Last Modified: Thu, 17 Sep 2020 00:40:11 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396b5d5b8015ed284fc3af5c77ed01816a546687827825bfe05386368054aef`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 4.4 MB (4393929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e45fcccc72b22e143ed1422bf729c9fce9dbfc00c055dc9c65e4f793b645c0`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 1.3 MB (1263460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0489d33a54da29f4c42f1172503ccf473a7fc8a053399c09f2b3edf6f1d9df7`  
		Last Modified: Thu, 17 Sep 2020 00:40:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56a47cc582b098f6e20069dc8198860e900c77ce25d2db40ccb0c594f8dba5`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 921.5 KB (921540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4973f508c3b66b7337bb4b3e98d55034788588cce9c5695f331c12d6ecfa80e7`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8aa1efe45d8600b6dd43c3af2cb754705b788f3a4ed6fe922524718bd6ffd7`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38364e96b8d00ce04bb18616ebf35caff24bcb161b689f1328d079c027de842f`  
		Last Modified: Thu, 17 Sep 2020 00:40:59 GMT  
		Size: 75.5 MB (75469512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250586f071176b3fd8b4b175100555ef49374cc44a6d2fecd0558edd9bbbd12b`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43caeb9b4c4a8bf3483b65d6d26c4e5667dff30c9464e8f20667e04bdb4f543c`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1` - linux; ppc64le

```console
$ docker pull mariadb@sha256:53458efa227fdc2c11f78350504dd9a3e765bdc99ef746ed0e23306e2b9f50ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118219224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524d74c3e832673dba181ae8e4b4662546e44f4dd30d4818e5f6403af8791b08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:29:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:32:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:32:40 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:34:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:35:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:35:02 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:35:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:40:49 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 19 Aug 2020 23:40:59 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Wed, 19 Aug 2020 23:41:23 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:46:43 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:47:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:47:05 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:47:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:47:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:47:27 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:47:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab250ae06399c73cc9817f3789a74adae8793413fbf0b3dbc4044f1f293039c5`  
		Last Modified: Wed, 19 Aug 2020 23:50:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e7708aae6e8ce6f8caaf4ffa1622806d8d0cab8d6f863465eb8c57d24ff017`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 5.6 MB (5629118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bf4f7913d267035e577ef35a10c655679701bac311e59d03642e6031119f9`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 1.2 MB (1246616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0fc286fe87be9ba7c7e3251b038029d16b999298ffa679d9b4bee3a322fac`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0ade7f823b839c6a7b8c54d586f05084d19d459d590f8edfb5546e18b40b55`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 932.0 KB (932036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a56b6d1750ce1842f6cdbfbe585bc1b5e08016cd10c8b10cfa8094760d53f`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2340f48aabe2adbb83a6ea5a463f1f8138ebc14ea7d2e259963199fa20d316e4`  
		Last Modified: Wed, 19 Aug 2020 23:51:03 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da5fc612041c19375d415742723258f7c69f5713bca40ed5a44c3ced2eb4d7`  
		Last Modified: Wed, 19 Aug 2020 23:51:21 GMT  
		Size: 80.0 MB (79953607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587d38fa113c7d9dace45a4074fbbd58049a488a2a697f31b24fadd2a191cae8`  
		Last Modified: Wed, 19 Aug 2020 23:51:03 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffab3ce35111f11c43f60616a3f77ba817dee4d49637291ee99f9b7d76dee98`  
		Last Modified: Wed, 19 Aug 2020 23:51:02 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.46`

```console
$ docker pull mariadb@sha256:6a7a45fa10c744a1fb821752709c406eed8f052a1a8b9ffec3ae3b78dfd5e619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.46` - linux; amd64

```console
$ docker pull mariadb@sha256:7712c5934462abd07b99753aeaad1b9d8db2332dc7da4264f292eebdadea9704
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113148337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:527f5e309b3de1640a11b17eea4366e2022f1b061fb85852621526d41922ab07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:11:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:11:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:11:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:11:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:11:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:32 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:11:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:12:20 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 17 Sep 2020 01:12:21 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Thu, 17 Sep 2020 01:12:21 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:13:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:13:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:13:06 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:13:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:13:07 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:13:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f302da1b612e8ea54850ec0495a374591b0a29677b6865b818490e1719d9fb`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8bf7c35412b355aaca3905c5d7ef2fd4800259be8ab1d2e7d7efa10857fedf`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 4.8 MB (4808571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324bc11a79a13859b04f667c46398832e8999729d311baed91fafc4008a4a52`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 1.3 MB (1326776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18579ec799327186b20c4ef266da0a3525f64343fefb0ea42b83568c1105c9c4`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de698a84499ad8d094edc88ede9c98efc6034c0f3dcd912916dd1d70a83f8dc6`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 930.0 KB (929998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ca9a2454258f016d19ebae1002aebd8e37b9d4dcc6a0bae0297143cf38910`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb349b72e6610d8d0078ef1077cfbbabb1857b96c7e39de299f3aa190e56915`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c42bb71bd12576c002e2043e5f87da3fa85d0cfa50fef11b19c854986b4f55`  
		Last Modified: Thu, 17 Sep 2020 01:15:13 GMT  
		Size: 79.4 MB (79369702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977bf6f7448ac99df7ce703fdfe6330842b49a2ab641f8332cf9b01475944fd`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a964f64afb85588c9daed5f65a65a9497d1a02e508241777c4b11fc2620623b`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.46` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:71266690948f44780ba1f3e9c48ca82c8f0f034c96c0b5bcb2d837d6a9b7f6bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105784494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9136f012257112f7d85a74fa68bf8a555980ad4ae3d12925df88b2a6c2e3cb8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:37 GMT
ADD file:9eedc88c2028d53a81210b52c98121dddea7e30ecfbd4d11d2a1b2bdc94a0102 in / 
# Wed, 16 Sep 2020 23:16:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:16:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:16:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:16:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:34:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:35:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:35:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:35:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:35:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:35:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:36:48 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 17 Sep 2020 00:36:48 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Thu, 17 Sep 2020 00:36:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:37:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:37:42 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:37:43 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:37:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:37:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:37:46 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:37:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2d8ee3976bc7c15c8a5279cdf0249b7e41b2a489771330d0f7affb26dd7acfb`  
		Last Modified: Fri, 04 Sep 2020 00:25:25 GMT  
		Size: 23.7 MB (23722305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007857f7b9b52d6efdfea9e086e6eaf35519130ff97bfe89970353f0ae53f13`  
		Last Modified: Wed, 16 Sep 2020 23:18:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43927e60f12d8b877ded6af5048b2ac5753fe78caba77a6bbbece4f98559b672`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d2e1ff6404f50b7e1c8366fc1c273c5b42cd576f7383176c3e65264aeebf5a`  
		Last Modified: Thu, 17 Sep 2020 00:40:11 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396b5d5b8015ed284fc3af5c77ed01816a546687827825bfe05386368054aef`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 4.4 MB (4393929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e45fcccc72b22e143ed1422bf729c9fce9dbfc00c055dc9c65e4f793b645c0`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 1.3 MB (1263460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0489d33a54da29f4c42f1172503ccf473a7fc8a053399c09f2b3edf6f1d9df7`  
		Last Modified: Thu, 17 Sep 2020 00:40:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56a47cc582b098f6e20069dc8198860e900c77ce25d2db40ccb0c594f8dba5`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 921.5 KB (921540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4973f508c3b66b7337bb4b3e98d55034788588cce9c5695f331c12d6ecfa80e7`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8aa1efe45d8600b6dd43c3af2cb754705b788f3a4ed6fe922524718bd6ffd7`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38364e96b8d00ce04bb18616ebf35caff24bcb161b689f1328d079c027de842f`  
		Last Modified: Thu, 17 Sep 2020 00:40:59 GMT  
		Size: 75.5 MB (75469512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250586f071176b3fd8b4b175100555ef49374cc44a6d2fecd0558edd9bbbd12b`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43caeb9b4c4a8bf3483b65d6d26c4e5667dff30c9464e8f20667e04bdb4f543c`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.46` - linux; ppc64le

```console
$ docker pull mariadb@sha256:53458efa227fdc2c11f78350504dd9a3e765bdc99ef746ed0e23306e2b9f50ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118219224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524d74c3e832673dba181ae8e4b4662546e44f4dd30d4818e5f6403af8791b08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:29:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:32:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:32:40 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:34:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:35:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:35:02 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:35:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:40:49 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 19 Aug 2020 23:40:59 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Wed, 19 Aug 2020 23:41:23 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:46:43 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:47:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:47:05 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:47:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:47:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:47:27 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:47:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab250ae06399c73cc9817f3789a74adae8793413fbf0b3dbc4044f1f293039c5`  
		Last Modified: Wed, 19 Aug 2020 23:50:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e7708aae6e8ce6f8caaf4ffa1622806d8d0cab8d6f863465eb8c57d24ff017`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 5.6 MB (5629118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bf4f7913d267035e577ef35a10c655679701bac311e59d03642e6031119f9`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 1.2 MB (1246616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0fc286fe87be9ba7c7e3251b038029d16b999298ffa679d9b4bee3a322fac`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0ade7f823b839c6a7b8c54d586f05084d19d459d590f8edfb5546e18b40b55`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 932.0 KB (932036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a56b6d1750ce1842f6cdbfbe585bc1b5e08016cd10c8b10cfa8094760d53f`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2340f48aabe2adbb83a6ea5a463f1f8138ebc14ea7d2e259963199fa20d316e4`  
		Last Modified: Wed, 19 Aug 2020 23:51:03 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da5fc612041c19375d415742723258f7c69f5713bca40ed5a44c3ced2eb4d7`  
		Last Modified: Wed, 19 Aug 2020 23:51:21 GMT  
		Size: 80.0 MB (79953607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587d38fa113c7d9dace45a4074fbbd58049a488a2a697f31b24fadd2a191cae8`  
		Last Modified: Wed, 19 Aug 2020 23:51:03 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffab3ce35111f11c43f60616a3f77ba817dee4d49637291ee99f9b7d76dee98`  
		Last Modified: Wed, 19 Aug 2020 23:51:02 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1.46-bionic`

```console
$ docker pull mariadb@sha256:6a7a45fa10c744a1fb821752709c406eed8f052a1a8b9ffec3ae3b78dfd5e619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1.46-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:7712c5934462abd07b99753aeaad1b9d8db2332dc7da4264f292eebdadea9704
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113148337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:527f5e309b3de1640a11b17eea4366e2022f1b061fb85852621526d41922ab07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:11:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:11:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:11:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:11:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:11:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:32 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:11:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:12:20 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 17 Sep 2020 01:12:21 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Thu, 17 Sep 2020 01:12:21 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:13:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:13:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:13:06 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:13:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:13:07 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:13:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f302da1b612e8ea54850ec0495a374591b0a29677b6865b818490e1719d9fb`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8bf7c35412b355aaca3905c5d7ef2fd4800259be8ab1d2e7d7efa10857fedf`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 4.8 MB (4808571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324bc11a79a13859b04f667c46398832e8999729d311baed91fafc4008a4a52`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 1.3 MB (1326776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18579ec799327186b20c4ef266da0a3525f64343fefb0ea42b83568c1105c9c4`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de698a84499ad8d094edc88ede9c98efc6034c0f3dcd912916dd1d70a83f8dc6`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 930.0 KB (929998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ca9a2454258f016d19ebae1002aebd8e37b9d4dcc6a0bae0297143cf38910`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb349b72e6610d8d0078ef1077cfbbabb1857b96c7e39de299f3aa190e56915`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c42bb71bd12576c002e2043e5f87da3fa85d0cfa50fef11b19c854986b4f55`  
		Last Modified: Thu, 17 Sep 2020 01:15:13 GMT  
		Size: 79.4 MB (79369702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977bf6f7448ac99df7ce703fdfe6330842b49a2ab641f8332cf9b01475944fd`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a964f64afb85588c9daed5f65a65a9497d1a02e508241777c4b11fc2620623b`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.46-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:71266690948f44780ba1f3e9c48ca82c8f0f034c96c0b5bcb2d837d6a9b7f6bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105784494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9136f012257112f7d85a74fa68bf8a555980ad4ae3d12925df88b2a6c2e3cb8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:37 GMT
ADD file:9eedc88c2028d53a81210b52c98121dddea7e30ecfbd4d11d2a1b2bdc94a0102 in / 
# Wed, 16 Sep 2020 23:16:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:16:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:16:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:16:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:34:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:35:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:35:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:35:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:35:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:35:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:36:48 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 17 Sep 2020 00:36:48 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Thu, 17 Sep 2020 00:36:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:37:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:37:42 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:37:43 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:37:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:37:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:37:46 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:37:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2d8ee3976bc7c15c8a5279cdf0249b7e41b2a489771330d0f7affb26dd7acfb`  
		Last Modified: Fri, 04 Sep 2020 00:25:25 GMT  
		Size: 23.7 MB (23722305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007857f7b9b52d6efdfea9e086e6eaf35519130ff97bfe89970353f0ae53f13`  
		Last Modified: Wed, 16 Sep 2020 23:18:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43927e60f12d8b877ded6af5048b2ac5753fe78caba77a6bbbece4f98559b672`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d2e1ff6404f50b7e1c8366fc1c273c5b42cd576f7383176c3e65264aeebf5a`  
		Last Modified: Thu, 17 Sep 2020 00:40:11 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396b5d5b8015ed284fc3af5c77ed01816a546687827825bfe05386368054aef`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 4.4 MB (4393929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e45fcccc72b22e143ed1422bf729c9fce9dbfc00c055dc9c65e4f793b645c0`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 1.3 MB (1263460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0489d33a54da29f4c42f1172503ccf473a7fc8a053399c09f2b3edf6f1d9df7`  
		Last Modified: Thu, 17 Sep 2020 00:40:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56a47cc582b098f6e20069dc8198860e900c77ce25d2db40ccb0c594f8dba5`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 921.5 KB (921540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4973f508c3b66b7337bb4b3e98d55034788588cce9c5695f331c12d6ecfa80e7`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8aa1efe45d8600b6dd43c3af2cb754705b788f3a4ed6fe922524718bd6ffd7`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38364e96b8d00ce04bb18616ebf35caff24bcb161b689f1328d079c027de842f`  
		Last Modified: Thu, 17 Sep 2020 00:40:59 GMT  
		Size: 75.5 MB (75469512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250586f071176b3fd8b4b175100555ef49374cc44a6d2fecd0558edd9bbbd12b`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43caeb9b4c4a8bf3483b65d6d26c4e5667dff30c9464e8f20667e04bdb4f543c`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1.46-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:53458efa227fdc2c11f78350504dd9a3e765bdc99ef746ed0e23306e2b9f50ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118219224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524d74c3e832673dba181ae8e4b4662546e44f4dd30d4818e5f6403af8791b08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:29:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:32:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:32:40 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:34:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:35:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:35:02 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:35:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:40:49 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 19 Aug 2020 23:40:59 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Wed, 19 Aug 2020 23:41:23 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:46:43 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:47:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:47:05 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:47:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:47:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:47:27 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:47:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab250ae06399c73cc9817f3789a74adae8793413fbf0b3dbc4044f1f293039c5`  
		Last Modified: Wed, 19 Aug 2020 23:50:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e7708aae6e8ce6f8caaf4ffa1622806d8d0cab8d6f863465eb8c57d24ff017`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 5.6 MB (5629118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bf4f7913d267035e577ef35a10c655679701bac311e59d03642e6031119f9`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 1.2 MB (1246616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0fc286fe87be9ba7c7e3251b038029d16b999298ffa679d9b4bee3a322fac`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0ade7f823b839c6a7b8c54d586f05084d19d459d590f8edfb5546e18b40b55`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 932.0 KB (932036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a56b6d1750ce1842f6cdbfbe585bc1b5e08016cd10c8b10cfa8094760d53f`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2340f48aabe2adbb83a6ea5a463f1f8138ebc14ea7d2e259963199fa20d316e4`  
		Last Modified: Wed, 19 Aug 2020 23:51:03 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da5fc612041c19375d415742723258f7c69f5713bca40ed5a44c3ced2eb4d7`  
		Last Modified: Wed, 19 Aug 2020 23:51:21 GMT  
		Size: 80.0 MB (79953607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587d38fa113c7d9dace45a4074fbbd58049a488a2a697f31b24fadd2a191cae8`  
		Last Modified: Wed, 19 Aug 2020 23:51:03 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffab3ce35111f11c43f60616a3f77ba817dee4d49637291ee99f9b7d76dee98`  
		Last Modified: Wed, 19 Aug 2020 23:51:02 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.1-bionic`

```console
$ docker pull mariadb@sha256:6a7a45fa10c744a1fb821752709c406eed8f052a1a8b9ffec3ae3b78dfd5e619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.1-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:7712c5934462abd07b99753aeaad1b9d8db2332dc7da4264f292eebdadea9704
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113148337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:527f5e309b3de1640a11b17eea4366e2022f1b061fb85852621526d41922ab07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:11:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:11:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:11:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:11:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:11:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:32 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:11:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:12:20 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 17 Sep 2020 01:12:21 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Thu, 17 Sep 2020 01:12:21 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:13:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:13:06 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:13:06 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:13:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:13:07 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:13:07 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f302da1b612e8ea54850ec0495a374591b0a29677b6865b818490e1719d9fb`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8bf7c35412b355aaca3905c5d7ef2fd4800259be8ab1d2e7d7efa10857fedf`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 4.8 MB (4808571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324bc11a79a13859b04f667c46398832e8999729d311baed91fafc4008a4a52`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 1.3 MB (1326776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18579ec799327186b20c4ef266da0a3525f64343fefb0ea42b83568c1105c9c4`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de698a84499ad8d094edc88ede9c98efc6034c0f3dcd912916dd1d70a83f8dc6`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 930.0 KB (929998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ca9a2454258f016d19ebae1002aebd8e37b9d4dcc6a0bae0297143cf38910`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb349b72e6610d8d0078ef1077cfbbabb1857b96c7e39de299f3aa190e56915`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c42bb71bd12576c002e2043e5f87da3fa85d0cfa50fef11b19c854986b4f55`  
		Last Modified: Thu, 17 Sep 2020 01:15:13 GMT  
		Size: 79.4 MB (79369702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e977bf6f7448ac99df7ce703fdfe6330842b49a2ab641f8332cf9b01475944fd`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a964f64afb85588c9daed5f65a65a9497d1a02e508241777c4b11fc2620623b`  
		Last Modified: Thu, 17 Sep 2020 01:14:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:71266690948f44780ba1f3e9c48ca82c8f0f034c96c0b5bcb2d837d6a9b7f6bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105784494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9136f012257112f7d85a74fa68bf8a555980ad4ae3d12925df88b2a6c2e3cb8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:37 GMT
ADD file:9eedc88c2028d53a81210b52c98121dddea7e30ecfbd4d11d2a1b2bdc94a0102 in / 
# Wed, 16 Sep 2020 23:16:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:16:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:16:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:16:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:34:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:35:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:35:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:35:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:35:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:35:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:36:48 GMT
ENV MARIADB_MAJOR=10.1
# Thu, 17 Sep 2020 00:36:48 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Thu, 17 Sep 2020 00:36:50 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:37:40 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:37:42 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:37:43 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:37:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:37:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:37:46 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:37:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2d8ee3976bc7c15c8a5279cdf0249b7e41b2a489771330d0f7affb26dd7acfb`  
		Last Modified: Fri, 04 Sep 2020 00:25:25 GMT  
		Size: 23.7 MB (23722305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007857f7b9b52d6efdfea9e086e6eaf35519130ff97bfe89970353f0ae53f13`  
		Last Modified: Wed, 16 Sep 2020 23:18:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43927e60f12d8b877ded6af5048b2ac5753fe78caba77a6bbbece4f98559b672`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d2e1ff6404f50b7e1c8366fc1c273c5b42cd576f7383176c3e65264aeebf5a`  
		Last Modified: Thu, 17 Sep 2020 00:40:11 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396b5d5b8015ed284fc3af5c77ed01816a546687827825bfe05386368054aef`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 4.4 MB (4393929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e45fcccc72b22e143ed1422bf729c9fce9dbfc00c055dc9c65e4f793b645c0`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 1.3 MB (1263460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0489d33a54da29f4c42f1172503ccf473a7fc8a053399c09f2b3edf6f1d9df7`  
		Last Modified: Thu, 17 Sep 2020 00:40:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56a47cc582b098f6e20069dc8198860e900c77ce25d2db40ccb0c594f8dba5`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 921.5 KB (921540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4973f508c3b66b7337bb4b3e98d55034788588cce9c5695f331c12d6ecfa80e7`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8aa1efe45d8600b6dd43c3af2cb754705b788f3a4ed6fe922524718bd6ffd7`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38364e96b8d00ce04bb18616ebf35caff24bcb161b689f1328d079c027de842f`  
		Last Modified: Thu, 17 Sep 2020 00:40:59 GMT  
		Size: 75.5 MB (75469512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250586f071176b3fd8b4b175100555ef49374cc44a6d2fecd0558edd9bbbd12b`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43caeb9b4c4a8bf3483b65d6d26c4e5667dff30c9464e8f20667e04bdb4f543c`  
		Last Modified: Thu, 17 Sep 2020 00:40:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.1-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:53458efa227fdc2c11f78350504dd9a3e765bdc99ef746ed0e23306e2b9f50ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118219224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:524d74c3e832673dba181ae8e4b4662546e44f4dd30d4818e5f6403af8791b08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:29:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:32:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:32:40 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:34:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:35:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:35:02 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:35:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:40:49 GMT
ENV MARIADB_MAJOR=10.1
# Wed, 19 Aug 2020 23:40:59 GMT
ENV MARIADB_VERSION=1:10.1.46+maria-1~bionic
# Wed, 19 Aug 2020 23:41:23 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:46:43 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.1 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:47:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:47:05 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:47:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:47:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:47:27 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:47:35 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab250ae06399c73cc9817f3789a74adae8793413fbf0b3dbc4044f1f293039c5`  
		Last Modified: Wed, 19 Aug 2020 23:50:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e7708aae6e8ce6f8caaf4ffa1622806d8d0cab8d6f863465eb8c57d24ff017`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 5.6 MB (5629118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bf4f7913d267035e577ef35a10c655679701bac311e59d03642e6031119f9`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 1.2 MB (1246616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0fc286fe87be9ba7c7e3251b038029d16b999298ffa679d9b4bee3a322fac`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0ade7f823b839c6a7b8c54d586f05084d19d459d590f8edfb5546e18b40b55`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 932.0 KB (932036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a56b6d1750ce1842f6cdbfbe585bc1b5e08016cd10c8b10cfa8094760d53f`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2340f48aabe2adbb83a6ea5a463f1f8138ebc14ea7d2e259963199fa20d316e4`  
		Last Modified: Wed, 19 Aug 2020 23:51:03 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4da5fc612041c19375d415742723258f7c69f5713bca40ed5a44c3ced2eb4d7`  
		Last Modified: Wed, 19 Aug 2020 23:51:21 GMT  
		Size: 80.0 MB (79953607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587d38fa113c7d9dace45a4074fbbd58049a488a2a697f31b24fadd2a191cae8`  
		Last Modified: Wed, 19 Aug 2020 23:51:03 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffab3ce35111f11c43f60616a3f77ba817dee4d49637291ee99f9b7d76dee98`  
		Last Modified: Wed, 19 Aug 2020 23:51:02 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2`

```console
$ docker pull mariadb@sha256:539f3799ce12157cb5cbd36c4eed811d5f1f7b8b082d8314ed8e5e912e4a8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2` - linux; amd64

```console
$ docker pull mariadb@sha256:18ca01b81342566f5153f8e5a4462b29878e3f6fe7d253dc5b106b5ec8961449
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109000132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9372439d1bcf89818b606fd19dfd9baebeb177ca78e254bc61ee65e24387f9ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:11:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:11:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:11:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:11:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:11:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:32 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:11:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:11:33 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 17 Sep 2020 01:11:33 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Thu, 17 Sep 2020 01:11:34 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:12:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:12:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:12:04 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:12:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:12:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:12:05 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:12:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f302da1b612e8ea54850ec0495a374591b0a29677b6865b818490e1719d9fb`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8bf7c35412b355aaca3905c5d7ef2fd4800259be8ab1d2e7d7efa10857fedf`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 4.8 MB (4808571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324bc11a79a13859b04f667c46398832e8999729d311baed91fafc4008a4a52`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 1.3 MB (1326776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18579ec799327186b20c4ef266da0a3525f64343fefb0ea42b83568c1105c9c4`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de698a84499ad8d094edc88ede9c98efc6034c0f3dcd912916dd1d70a83f8dc6`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 930.0 KB (929998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ca9a2454258f016d19ebae1002aebd8e37b9d4dcc6a0bae0297143cf38910`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6067b1a2052deb8d27465b8cf6325d371d2af1cc16d30deab704b6c10078f965`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1327450532aced721f6d247328be2dadb434df6cad784538c9f17882a5eddf`  
		Last Modified: Thu, 17 Sep 2020 01:14:52 GMT  
		Size: 75.2 MB (75221496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbf6872bd3e301cd921ef0f331a4780fffe77f8f8bd4b4e7e4d3f96c3ffa61f`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c66153a1e46b9798d529c16a33ed899ad8bf4ed176f605ada4c9c5da928ed9`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:baf8d6eee73818c3d97291ac2da237d2424e42305bc3f6fdc1b90e026efe0b3b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104059297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a87749f40e0f01ec26ad1e8038d62bfe9fd806a2a90d1aa89eaeee23b58c292`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:37 GMT
ADD file:9eedc88c2028d53a81210b52c98121dddea7e30ecfbd4d11d2a1b2bdc94a0102 in / 
# Wed, 16 Sep 2020 23:16:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:16:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:16:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:16:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:34:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:35:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:35:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:35:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:35:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:35:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:35:44 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 17 Sep 2020 00:35:44 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Thu, 17 Sep 2020 00:35:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:36:30 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:36:32 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:36:33 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:36:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:36:36 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:36:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2d8ee3976bc7c15c8a5279cdf0249b7e41b2a489771330d0f7affb26dd7acfb`  
		Last Modified: Fri, 04 Sep 2020 00:25:25 GMT  
		Size: 23.7 MB (23722305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007857f7b9b52d6efdfea9e086e6eaf35519130ff97bfe89970353f0ae53f13`  
		Last Modified: Wed, 16 Sep 2020 23:18:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43927e60f12d8b877ded6af5048b2ac5753fe78caba77a6bbbece4f98559b672`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d2e1ff6404f50b7e1c8366fc1c273c5b42cd576f7383176c3e65264aeebf5a`  
		Last Modified: Thu, 17 Sep 2020 00:40:11 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396b5d5b8015ed284fc3af5c77ed01816a546687827825bfe05386368054aef`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 4.4 MB (4393929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e45fcccc72b22e143ed1422bf729c9fce9dbfc00c055dc9c65e4f793b645c0`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 1.3 MB (1263460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0489d33a54da29f4c42f1172503ccf473a7fc8a053399c09f2b3edf6f1d9df7`  
		Last Modified: Thu, 17 Sep 2020 00:40:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56a47cc582b098f6e20069dc8198860e900c77ce25d2db40ccb0c594f8dba5`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 921.5 KB (921540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4973f508c3b66b7337bb4b3e98d55034788588cce9c5695f331c12d6ecfa80e7`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50026ad17eafe3b0ab0f2b71f3eac550285fd21571e793fee93a3146ee47dc91`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6212bee68bcab5b712b24899b27e3b78bed1bb32cb1b9e900c30cd4770abea3`  
		Last Modified: Thu, 17 Sep 2020 00:40:28 GMT  
		Size: 73.7 MB (73744319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949f3573df560acdc7d9e5b87b92379a46a85d38d2552e2f5020901e3b798f6`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa8b13de8157fee866ac8cc2f8c9734bcb6932d336a6b575d8e00beeb3fe185`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2` - linux; ppc64le

```console
$ docker pull mariadb@sha256:353edf79c1238d2dd16e1fb0718fc057d8ab62ed85410d95312835c3c75f65f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116269512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b281851dd6f52e2b8b64933867bf044b3f9d7827415819b8bfae2448ada5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:29:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:32:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:32:40 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:34:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:35:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:35:02 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:35:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:35:21 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 19 Aug 2020 23:35:28 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Wed, 19 Aug 2020 23:35:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:39:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:39:59 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:40:02 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:40:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:40:28 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:40:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab250ae06399c73cc9817f3789a74adae8793413fbf0b3dbc4044f1f293039c5`  
		Last Modified: Wed, 19 Aug 2020 23:50:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e7708aae6e8ce6f8caaf4ffa1622806d8d0cab8d6f863465eb8c57d24ff017`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 5.6 MB (5629118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bf4f7913d267035e577ef35a10c655679701bac311e59d03642e6031119f9`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 1.2 MB (1246616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0fc286fe87be9ba7c7e3251b038029d16b999298ffa679d9b4bee3a322fac`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0ade7f823b839c6a7b8c54d586f05084d19d459d590f8edfb5546e18b40b55`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 932.0 KB (932036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a56b6d1750ce1842f6cdbfbe585bc1b5e08016cd10c8b10cfa8094760d53f`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5206c520f6b5bdc4291b6687ddb584bd2f3f4160ef692045d78582be47eec7b8`  
		Last Modified: Wed, 19 Aug 2020 23:50:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2821d2861454e6bc035fc9db6c83fa719f4d38c6e49dfc2642e2b83d160386`  
		Last Modified: Wed, 19 Aug 2020 23:50:46 GMT  
		Size: 78.0 MB (78003891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72687dea1b5a65013f9a1ab8ef6d02e0308e8887623e083005d3b5ef8b350d8`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445d27348b28f71fb5c978f811b352b78a78e95c08ea761d3a59caeac307f661`  
		Last Modified: Wed, 19 Aug 2020 23:50:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.33`

```console
$ docker pull mariadb@sha256:539f3799ce12157cb5cbd36c4eed811d5f1f7b8b082d8314ed8e5e912e4a8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.33` - linux; amd64

```console
$ docker pull mariadb@sha256:18ca01b81342566f5153f8e5a4462b29878e3f6fe7d253dc5b106b5ec8961449
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109000132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9372439d1bcf89818b606fd19dfd9baebeb177ca78e254bc61ee65e24387f9ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:11:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:11:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:11:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:11:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:11:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:32 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:11:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:11:33 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 17 Sep 2020 01:11:33 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Thu, 17 Sep 2020 01:11:34 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:12:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:12:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:12:04 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:12:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:12:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:12:05 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:12:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f302da1b612e8ea54850ec0495a374591b0a29677b6865b818490e1719d9fb`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8bf7c35412b355aaca3905c5d7ef2fd4800259be8ab1d2e7d7efa10857fedf`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 4.8 MB (4808571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324bc11a79a13859b04f667c46398832e8999729d311baed91fafc4008a4a52`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 1.3 MB (1326776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18579ec799327186b20c4ef266da0a3525f64343fefb0ea42b83568c1105c9c4`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de698a84499ad8d094edc88ede9c98efc6034c0f3dcd912916dd1d70a83f8dc6`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 930.0 KB (929998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ca9a2454258f016d19ebae1002aebd8e37b9d4dcc6a0bae0297143cf38910`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6067b1a2052deb8d27465b8cf6325d371d2af1cc16d30deab704b6c10078f965`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1327450532aced721f6d247328be2dadb434df6cad784538c9f17882a5eddf`  
		Last Modified: Thu, 17 Sep 2020 01:14:52 GMT  
		Size: 75.2 MB (75221496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbf6872bd3e301cd921ef0f331a4780fffe77f8f8bd4b4e7e4d3f96c3ffa61f`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c66153a1e46b9798d529c16a33ed899ad8bf4ed176f605ada4c9c5da928ed9`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.33` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:baf8d6eee73818c3d97291ac2da237d2424e42305bc3f6fdc1b90e026efe0b3b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104059297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a87749f40e0f01ec26ad1e8038d62bfe9fd806a2a90d1aa89eaeee23b58c292`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:37 GMT
ADD file:9eedc88c2028d53a81210b52c98121dddea7e30ecfbd4d11d2a1b2bdc94a0102 in / 
# Wed, 16 Sep 2020 23:16:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:16:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:16:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:16:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:34:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:35:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:35:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:35:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:35:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:35:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:35:44 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 17 Sep 2020 00:35:44 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Thu, 17 Sep 2020 00:35:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:36:30 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:36:32 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:36:33 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:36:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:36:36 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:36:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2d8ee3976bc7c15c8a5279cdf0249b7e41b2a489771330d0f7affb26dd7acfb`  
		Last Modified: Fri, 04 Sep 2020 00:25:25 GMT  
		Size: 23.7 MB (23722305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007857f7b9b52d6efdfea9e086e6eaf35519130ff97bfe89970353f0ae53f13`  
		Last Modified: Wed, 16 Sep 2020 23:18:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43927e60f12d8b877ded6af5048b2ac5753fe78caba77a6bbbece4f98559b672`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d2e1ff6404f50b7e1c8366fc1c273c5b42cd576f7383176c3e65264aeebf5a`  
		Last Modified: Thu, 17 Sep 2020 00:40:11 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396b5d5b8015ed284fc3af5c77ed01816a546687827825bfe05386368054aef`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 4.4 MB (4393929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e45fcccc72b22e143ed1422bf729c9fce9dbfc00c055dc9c65e4f793b645c0`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 1.3 MB (1263460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0489d33a54da29f4c42f1172503ccf473a7fc8a053399c09f2b3edf6f1d9df7`  
		Last Modified: Thu, 17 Sep 2020 00:40:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56a47cc582b098f6e20069dc8198860e900c77ce25d2db40ccb0c594f8dba5`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 921.5 KB (921540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4973f508c3b66b7337bb4b3e98d55034788588cce9c5695f331c12d6ecfa80e7`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50026ad17eafe3b0ab0f2b71f3eac550285fd21571e793fee93a3146ee47dc91`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6212bee68bcab5b712b24899b27e3b78bed1bb32cb1b9e900c30cd4770abea3`  
		Last Modified: Thu, 17 Sep 2020 00:40:28 GMT  
		Size: 73.7 MB (73744319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949f3573df560acdc7d9e5b87b92379a46a85d38d2552e2f5020901e3b798f6`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa8b13de8157fee866ac8cc2f8c9734bcb6932d336a6b575d8e00beeb3fe185`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.33` - linux; ppc64le

```console
$ docker pull mariadb@sha256:353edf79c1238d2dd16e1fb0718fc057d8ab62ed85410d95312835c3c75f65f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116269512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b281851dd6f52e2b8b64933867bf044b3f9d7827415819b8bfae2448ada5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:29:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:32:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:32:40 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:34:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:35:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:35:02 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:35:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:35:21 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 19 Aug 2020 23:35:28 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Wed, 19 Aug 2020 23:35:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:39:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:39:59 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:40:02 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:40:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:40:28 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:40:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab250ae06399c73cc9817f3789a74adae8793413fbf0b3dbc4044f1f293039c5`  
		Last Modified: Wed, 19 Aug 2020 23:50:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e7708aae6e8ce6f8caaf4ffa1622806d8d0cab8d6f863465eb8c57d24ff017`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 5.6 MB (5629118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bf4f7913d267035e577ef35a10c655679701bac311e59d03642e6031119f9`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 1.2 MB (1246616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0fc286fe87be9ba7c7e3251b038029d16b999298ffa679d9b4bee3a322fac`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0ade7f823b839c6a7b8c54d586f05084d19d459d590f8edfb5546e18b40b55`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 932.0 KB (932036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a56b6d1750ce1842f6cdbfbe585bc1b5e08016cd10c8b10cfa8094760d53f`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5206c520f6b5bdc4291b6687ddb584bd2f3f4160ef692045d78582be47eec7b8`  
		Last Modified: Wed, 19 Aug 2020 23:50:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2821d2861454e6bc035fc9db6c83fa719f4d38c6e49dfc2642e2b83d160386`  
		Last Modified: Wed, 19 Aug 2020 23:50:46 GMT  
		Size: 78.0 MB (78003891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72687dea1b5a65013f9a1ab8ef6d02e0308e8887623e083005d3b5ef8b350d8`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445d27348b28f71fb5c978f811b352b78a78e95c08ea761d3a59caeac307f661`  
		Last Modified: Wed, 19 Aug 2020 23:50:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2.33-bionic`

```console
$ docker pull mariadb@sha256:539f3799ce12157cb5cbd36c4eed811d5f1f7b8b082d8314ed8e5e912e4a8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2.33-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:18ca01b81342566f5153f8e5a4462b29878e3f6fe7d253dc5b106b5ec8961449
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109000132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9372439d1bcf89818b606fd19dfd9baebeb177ca78e254bc61ee65e24387f9ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:11:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:11:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:11:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:11:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:11:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:32 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:11:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:11:33 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 17 Sep 2020 01:11:33 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Thu, 17 Sep 2020 01:11:34 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:12:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:12:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:12:04 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:12:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:12:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:12:05 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:12:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f302da1b612e8ea54850ec0495a374591b0a29677b6865b818490e1719d9fb`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8bf7c35412b355aaca3905c5d7ef2fd4800259be8ab1d2e7d7efa10857fedf`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 4.8 MB (4808571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324bc11a79a13859b04f667c46398832e8999729d311baed91fafc4008a4a52`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 1.3 MB (1326776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18579ec799327186b20c4ef266da0a3525f64343fefb0ea42b83568c1105c9c4`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de698a84499ad8d094edc88ede9c98efc6034c0f3dcd912916dd1d70a83f8dc6`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 930.0 KB (929998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ca9a2454258f016d19ebae1002aebd8e37b9d4dcc6a0bae0297143cf38910`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6067b1a2052deb8d27465b8cf6325d371d2af1cc16d30deab704b6c10078f965`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1327450532aced721f6d247328be2dadb434df6cad784538c9f17882a5eddf`  
		Last Modified: Thu, 17 Sep 2020 01:14:52 GMT  
		Size: 75.2 MB (75221496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbf6872bd3e301cd921ef0f331a4780fffe77f8f8bd4b4e7e4d3f96c3ffa61f`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c66153a1e46b9798d529c16a33ed899ad8bf4ed176f605ada4c9c5da928ed9`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.33-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:baf8d6eee73818c3d97291ac2da237d2424e42305bc3f6fdc1b90e026efe0b3b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104059297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a87749f40e0f01ec26ad1e8038d62bfe9fd806a2a90d1aa89eaeee23b58c292`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:37 GMT
ADD file:9eedc88c2028d53a81210b52c98121dddea7e30ecfbd4d11d2a1b2bdc94a0102 in / 
# Wed, 16 Sep 2020 23:16:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:16:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:16:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:16:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:34:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:35:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:35:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:35:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:35:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:35:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:35:44 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 17 Sep 2020 00:35:44 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Thu, 17 Sep 2020 00:35:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:36:30 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:36:32 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:36:33 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:36:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:36:36 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:36:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2d8ee3976bc7c15c8a5279cdf0249b7e41b2a489771330d0f7affb26dd7acfb`  
		Last Modified: Fri, 04 Sep 2020 00:25:25 GMT  
		Size: 23.7 MB (23722305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007857f7b9b52d6efdfea9e086e6eaf35519130ff97bfe89970353f0ae53f13`  
		Last Modified: Wed, 16 Sep 2020 23:18:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43927e60f12d8b877ded6af5048b2ac5753fe78caba77a6bbbece4f98559b672`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d2e1ff6404f50b7e1c8366fc1c273c5b42cd576f7383176c3e65264aeebf5a`  
		Last Modified: Thu, 17 Sep 2020 00:40:11 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396b5d5b8015ed284fc3af5c77ed01816a546687827825bfe05386368054aef`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 4.4 MB (4393929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e45fcccc72b22e143ed1422bf729c9fce9dbfc00c055dc9c65e4f793b645c0`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 1.3 MB (1263460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0489d33a54da29f4c42f1172503ccf473a7fc8a053399c09f2b3edf6f1d9df7`  
		Last Modified: Thu, 17 Sep 2020 00:40:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56a47cc582b098f6e20069dc8198860e900c77ce25d2db40ccb0c594f8dba5`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 921.5 KB (921540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4973f508c3b66b7337bb4b3e98d55034788588cce9c5695f331c12d6ecfa80e7`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50026ad17eafe3b0ab0f2b71f3eac550285fd21571e793fee93a3146ee47dc91`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6212bee68bcab5b712b24899b27e3b78bed1bb32cb1b9e900c30cd4770abea3`  
		Last Modified: Thu, 17 Sep 2020 00:40:28 GMT  
		Size: 73.7 MB (73744319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949f3573df560acdc7d9e5b87b92379a46a85d38d2552e2f5020901e3b798f6`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa8b13de8157fee866ac8cc2f8c9734bcb6932d336a6b575d8e00beeb3fe185`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2.33-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:353edf79c1238d2dd16e1fb0718fc057d8ab62ed85410d95312835c3c75f65f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116269512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b281851dd6f52e2b8b64933867bf044b3f9d7827415819b8bfae2448ada5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:29:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:32:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:32:40 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:34:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:35:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:35:02 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:35:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:35:21 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 19 Aug 2020 23:35:28 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Wed, 19 Aug 2020 23:35:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:39:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:39:59 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:40:02 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:40:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:40:28 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:40:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab250ae06399c73cc9817f3789a74adae8793413fbf0b3dbc4044f1f293039c5`  
		Last Modified: Wed, 19 Aug 2020 23:50:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e7708aae6e8ce6f8caaf4ffa1622806d8d0cab8d6f863465eb8c57d24ff017`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 5.6 MB (5629118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bf4f7913d267035e577ef35a10c655679701bac311e59d03642e6031119f9`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 1.2 MB (1246616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0fc286fe87be9ba7c7e3251b038029d16b999298ffa679d9b4bee3a322fac`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0ade7f823b839c6a7b8c54d586f05084d19d459d590f8edfb5546e18b40b55`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 932.0 KB (932036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a56b6d1750ce1842f6cdbfbe585bc1b5e08016cd10c8b10cfa8094760d53f`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5206c520f6b5bdc4291b6687ddb584bd2f3f4160ef692045d78582be47eec7b8`  
		Last Modified: Wed, 19 Aug 2020 23:50:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2821d2861454e6bc035fc9db6c83fa719f4d38c6e49dfc2642e2b83d160386`  
		Last Modified: Wed, 19 Aug 2020 23:50:46 GMT  
		Size: 78.0 MB (78003891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72687dea1b5a65013f9a1ab8ef6d02e0308e8887623e083005d3b5ef8b350d8`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445d27348b28f71fb5c978f811b352b78a78e95c08ea761d3a59caeac307f661`  
		Last Modified: Wed, 19 Aug 2020 23:50:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.2-bionic`

```console
$ docker pull mariadb@sha256:539f3799ce12157cb5cbd36c4eed811d5f1f7b8b082d8314ed8e5e912e4a8636
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.2-bionic` - linux; amd64

```console
$ docker pull mariadb@sha256:18ca01b81342566f5153f8e5a4462b29878e3f6fe7d253dc5b106b5ec8961449
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109000132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9372439d1bcf89818b606fd19dfd9baebeb177ca78e254bc61ee65e24387f9ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:02 GMT
ADD file:84f8ddc4d76e1e867ab084f300cf4c2397bb9e4628d83dc22f4f5e2f6ec670b4 in / 
# Wed, 16 Sep 2020 22:20:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:05 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:11:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:11:13 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:11:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:11:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:11:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:11:32 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:11:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:11:33 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 17 Sep 2020 01:11:33 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Thu, 17 Sep 2020 01:11:34 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:12:03 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:12:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:12:04 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:12:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:12:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:12:05 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:12:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d9821c948472065b3c166b4abc08367160961c9ac4639eb0023670ab4845a6a`  
		Last Modified: Fri, 04 Sep 2020 12:21:34 GMT  
		Size: 26.7 MB (26699608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a610eae58dfceafc0725cb0472249020f75bcc796468615798ee394cbaf86120`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40e0eb9f1408cd0bee02979b33f05689110bc9caba370388d94f73b46a6379a`  
		Last Modified: Wed, 16 Sep 2020 22:23:01 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f302da1b612e8ea54850ec0495a374591b0a29677b6865b818490e1719d9fb`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8bf7c35412b355aaca3905c5d7ef2fd4800259be8ab1d2e7d7efa10857fedf`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 4.8 MB (4808571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324bc11a79a13859b04f667c46398832e8999729d311baed91fafc4008a4a52`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 1.3 MB (1326776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18579ec799327186b20c4ef266da0a3525f64343fefb0ea42b83568c1105c9c4`  
		Last Modified: Thu, 17 Sep 2020 01:14:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de698a84499ad8d094edc88ede9c98efc6034c0f3dcd912916dd1d70a83f8dc6`  
		Last Modified: Thu, 17 Sep 2020 01:14:40 GMT  
		Size: 930.0 KB (929998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16ca9a2454258f016d19ebae1002aebd8e37b9d4dcc6a0bae0297143cf38910`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.2 KB (5170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6067b1a2052deb8d27465b8cf6325d371d2af1cc16d30deab704b6c10078f965`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1327450532aced721f6d247328be2dadb434df6cad784538c9f17882a5eddf`  
		Last Modified: Thu, 17 Sep 2020 01:14:52 GMT  
		Size: 75.2 MB (75221496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbf6872bd3e301cd921ef0f331a4780fffe77f8f8bd4b4e7e4d3f96c3ffa61f`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c66153a1e46b9798d529c16a33ed899ad8bf4ed176f605ada4c9c5da928ed9`  
		Last Modified: Thu, 17 Sep 2020 01:14:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:baf8d6eee73818c3d97291ac2da237d2424e42305bc3f6fdc1b90e026efe0b3b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.1 MB (104059297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a87749f40e0f01ec26ad1e8038d62bfe9fd806a2a90d1aa89eaeee23b58c292`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:37 GMT
ADD file:9eedc88c2028d53a81210b52c98121dddea7e30ecfbd4d11d2a1b2bdc94a0102 in / 
# Wed, 16 Sep 2020 23:16:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:16:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:16:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:16:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:34:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:35:06 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:08 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:35:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:35:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:35:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:35:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:35:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:35:44 GMT
ENV MARIADB_MAJOR=10.2
# Thu, 17 Sep 2020 00:35:44 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Thu, 17 Sep 2020 00:35:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:36:30 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:36:32 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:36:33 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:36:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:36:36 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:36:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e2d8ee3976bc7c15c8a5279cdf0249b7e41b2a489771330d0f7affb26dd7acfb`  
		Last Modified: Fri, 04 Sep 2020 00:25:25 GMT  
		Size: 23.7 MB (23722305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5007857f7b9b52d6efdfea9e086e6eaf35519130ff97bfe89970353f0ae53f13`  
		Last Modified: Wed, 16 Sep 2020 23:18:23 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43927e60f12d8b877ded6af5048b2ac5753fe78caba77a6bbbece4f98559b672`  
		Last Modified: Wed, 16 Sep 2020 23:18:22 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d2e1ff6404f50b7e1c8366fc1c273c5b42cd576f7383176c3e65264aeebf5a`  
		Last Modified: Thu, 17 Sep 2020 00:40:11 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396b5d5b8015ed284fc3af5c77ed01816a546687827825bfe05386368054aef`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 4.4 MB (4393929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e45fcccc72b22e143ed1422bf729c9fce9dbfc00c055dc9c65e4f793b645c0`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 1.3 MB (1263460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0489d33a54da29f4c42f1172503ccf473a7fc8a053399c09f2b3edf6f1d9df7`  
		Last Modified: Thu, 17 Sep 2020 00:40:08 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56a47cc582b098f6e20069dc8198860e900c77ce25d2db40ccb0c594f8dba5`  
		Last Modified: Thu, 17 Sep 2020 00:40:09 GMT  
		Size: 921.5 KB (921540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4973f508c3b66b7337bb4b3e98d55034788588cce9c5695f331c12d6ecfa80e7`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50026ad17eafe3b0ab0f2b71f3eac550285fd21571e793fee93a3146ee47dc91`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6212bee68bcab5b712b24899b27e3b78bed1bb32cb1b9e900c30cd4770abea3`  
		Last Modified: Thu, 17 Sep 2020 00:40:28 GMT  
		Size: 73.7 MB (73744319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949f3573df560acdc7d9e5b87b92379a46a85d38d2552e2f5020901e3b798f6`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa8b13de8157fee866ac8cc2f8c9734bcb6932d336a6b575d8e00beeb3fe185`  
		Last Modified: Thu, 17 Sep 2020 00:40:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.2-bionic` - linux; ppc64le

```console
$ docker pull mariadb@sha256:353edf79c1238d2dd16e1fb0718fc057d8ab62ed85410d95312835c3c75f65f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116269512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b281851dd6f52e2b8b64933867bf044b3f9d7827415819b8bfae2448ada5655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:29:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:32:34 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:32:40 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:34:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:34:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:35:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:35:02 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:35:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:35:21 GMT
ENV MARIADB_MAJOR=10.2
# Wed, 19 Aug 2020 23:35:28 GMT
ENV MARIADB_VERSION=1:10.2.33+maria~bionic
# Wed, 19 Aug 2020 23:35:44 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu bionic main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:39:46 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup-10.2 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:39:59 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:40:02 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:40:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:40:28 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:40:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab250ae06399c73cc9817f3789a74adae8793413fbf0b3dbc4044f1f293039c5`  
		Last Modified: Wed, 19 Aug 2020 23:50:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e7708aae6e8ce6f8caaf4ffa1622806d8d0cab8d6f863465eb8c57d24ff017`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 5.6 MB (5629118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44bf4f7913d267035e577ef35a10c655679701bac311e59d03642e6031119f9`  
		Last Modified: Wed, 19 Aug 2020 23:50:34 GMT  
		Size: 1.2 MB (1246616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b0fc286fe87be9ba7c7e3251b038029d16b999298ffa679d9b4bee3a322fac`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0ade7f823b839c6a7b8c54d586f05084d19d459d590f8edfb5546e18b40b55`  
		Last Modified: Wed, 19 Aug 2020 23:50:32 GMT  
		Size: 932.0 KB (932036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a56b6d1750ce1842f6cdbfbe585bc1b5e08016cd10c8b10cfa8094760d53f`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.2 KB (5173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5206c520f6b5bdc4291b6687ddb584bd2f3f4160ef692045d78582be47eec7b8`  
		Last Modified: Wed, 19 Aug 2020 23:50:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2821d2861454e6bc035fc9db6c83fa719f4d38c6e49dfc2642e2b83d160386`  
		Last Modified: Wed, 19 Aug 2020 23:50:46 GMT  
		Size: 78.0 MB (78003891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72687dea1b5a65013f9a1ab8ef6d02e0308e8887623e083005d3b5ef8b350d8`  
		Last Modified: Wed, 19 Aug 2020 23:50:27 GMT  
		Size: 5.1 KB (5058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445d27348b28f71fb5c978f811b352b78a78e95c08ea761d3a59caeac307f661`  
		Last Modified: Wed, 19 Aug 2020 23:50:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3`

```console
$ docker pull mariadb@sha256:bf94a1e968e256b0c8b13be4e2ce8f02266dd514361b31de5484734ee6b367d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3` - linux; amd64

```console
$ docker pull mariadb@sha256:07988d63348d04e66e3b78422ed0d47f561a59ebb38620fe25cb08241755a141
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119157984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16f787686dec1308849e08dd22202f038982cd934ba624f7a1b4b81d1c00bb75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:10:17 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 17 Sep 2020 01:10:17 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Thu, 17 Sep 2020 01:10:18 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:10:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:10:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:10:58 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:10:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:10:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:10:59 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:10:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420ae5e12220ef79c1f0cef0a708cb1b8ad217f4e595290a9aee6ebbb9943224`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7539ff915a5c293690d5f1321a7f729747c28beabc4ceee1480d885380a59c37`  
		Last Modified: Thu, 17 Sep 2020 01:14:32 GMT  
		Size: 82.5 MB (82512002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aee0e8778e20d8f3114bcaeceb4c0dd4d54a495665f21d495fa9f2bc956d69`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694594587433345707b0eb20693bae9924990a034bb41551ff32a25732dfae0c`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f6866f9b8c5c04bab5299827002b624a2b330010ce0fe1a3b9048d593068c87a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116815031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d7c574ae73596b744870667c1144f4d0b224c49ed45494fa679c3768a288b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:33:37 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 17 Sep 2020 00:33:38 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Thu, 17 Sep 2020 00:33:40 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:34:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:34:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:34:30 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:34:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:34:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:34:35 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:34:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2c304b19aabdb5b2d97c6cf9387086880a09dc307a28c01de5e729981b327`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1b7e546454a80634c5c004e80de39c5384331b724a6252a898710dfe070624`  
		Last Modified: Thu, 17 Sep 2020 00:39:50 GMT  
		Size: 81.7 MB (81663466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1369725b701991b582b2c14f6a8e4f46bcf1e2d2b0d34901ac164e4699a2f82c`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e071e3d1b3531c578027ef9c0140972c7112306c6c7c6cfbbb3ee36547bf1a05`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6ada9a72057b09698f940a19061ed21345c69de1638caf1ae7f6aebea55fd946
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129011810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be004206f8c63f53a64ff60d2bde11541c889278fa4d861eb4aee77718335d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:20:11 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 19 Aug 2020 23:20:23 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Wed, 19 Aug 2020 23:20:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:28:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:28:25 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:28:29 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:28:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:28:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:28:46 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:28:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f324cbd967ceab87e63252c88e75d723fe929ad23856787ac94973461a1f3499`  
		Last Modified: Wed, 19 Aug 2020 23:49:51 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daaecc0bb5f0b8aa41068b03046d09dd4b04aea298f52bc01fb614f78cb4a3d`  
		Last Modified: Wed, 19 Aug 2020 23:50:10 GMT  
		Size: 86.5 MB (86503749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240555122f3825796c16c25757b030eb667ffe353b470e0557462564512a17e9`  
		Last Modified: Wed, 19 Aug 2020 23:49:53 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea38786ce8caadcec478b7302a1bf2c2580eb82c1b40b17c1601c0f778b4a2`  
		Last Modified: Wed, 19 Aug 2020 23:49:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.24`

```console
$ docker pull mariadb@sha256:bf94a1e968e256b0c8b13be4e2ce8f02266dd514361b31de5484734ee6b367d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.24` - linux; amd64

```console
$ docker pull mariadb@sha256:07988d63348d04e66e3b78422ed0d47f561a59ebb38620fe25cb08241755a141
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119157984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16f787686dec1308849e08dd22202f038982cd934ba624f7a1b4b81d1c00bb75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:10:17 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 17 Sep 2020 01:10:17 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Thu, 17 Sep 2020 01:10:18 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:10:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:10:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:10:58 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:10:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:10:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:10:59 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:10:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420ae5e12220ef79c1f0cef0a708cb1b8ad217f4e595290a9aee6ebbb9943224`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7539ff915a5c293690d5f1321a7f729747c28beabc4ceee1480d885380a59c37`  
		Last Modified: Thu, 17 Sep 2020 01:14:32 GMT  
		Size: 82.5 MB (82512002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aee0e8778e20d8f3114bcaeceb4c0dd4d54a495665f21d495fa9f2bc956d69`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694594587433345707b0eb20693bae9924990a034bb41551ff32a25732dfae0c`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.24` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f6866f9b8c5c04bab5299827002b624a2b330010ce0fe1a3b9048d593068c87a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116815031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d7c574ae73596b744870667c1144f4d0b224c49ed45494fa679c3768a288b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:33:37 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 17 Sep 2020 00:33:38 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Thu, 17 Sep 2020 00:33:40 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:34:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:34:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:34:30 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:34:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:34:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:34:35 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:34:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2c304b19aabdb5b2d97c6cf9387086880a09dc307a28c01de5e729981b327`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1b7e546454a80634c5c004e80de39c5384331b724a6252a898710dfe070624`  
		Last Modified: Thu, 17 Sep 2020 00:39:50 GMT  
		Size: 81.7 MB (81663466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1369725b701991b582b2c14f6a8e4f46bcf1e2d2b0d34901ac164e4699a2f82c`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e071e3d1b3531c578027ef9c0140972c7112306c6c7c6cfbbb3ee36547bf1a05`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.24` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6ada9a72057b09698f940a19061ed21345c69de1638caf1ae7f6aebea55fd946
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129011810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be004206f8c63f53a64ff60d2bde11541c889278fa4d861eb4aee77718335d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:20:11 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 19 Aug 2020 23:20:23 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Wed, 19 Aug 2020 23:20:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:28:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:28:25 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:28:29 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:28:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:28:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:28:46 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:28:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f324cbd967ceab87e63252c88e75d723fe929ad23856787ac94973461a1f3499`  
		Last Modified: Wed, 19 Aug 2020 23:49:51 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daaecc0bb5f0b8aa41068b03046d09dd4b04aea298f52bc01fb614f78cb4a3d`  
		Last Modified: Wed, 19 Aug 2020 23:50:10 GMT  
		Size: 86.5 MB (86503749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240555122f3825796c16c25757b030eb667ffe353b470e0557462564512a17e9`  
		Last Modified: Wed, 19 Aug 2020 23:49:53 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea38786ce8caadcec478b7302a1bf2c2580eb82c1b40b17c1601c0f778b4a2`  
		Last Modified: Wed, 19 Aug 2020 23:49:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3.24-focal`

```console
$ docker pull mariadb@sha256:bf94a1e968e256b0c8b13be4e2ce8f02266dd514361b31de5484734ee6b367d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3.24-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:07988d63348d04e66e3b78422ed0d47f561a59ebb38620fe25cb08241755a141
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119157984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16f787686dec1308849e08dd22202f038982cd934ba624f7a1b4b81d1c00bb75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:10:17 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 17 Sep 2020 01:10:17 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Thu, 17 Sep 2020 01:10:18 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:10:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:10:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:10:58 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:10:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:10:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:10:59 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:10:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420ae5e12220ef79c1f0cef0a708cb1b8ad217f4e595290a9aee6ebbb9943224`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7539ff915a5c293690d5f1321a7f729747c28beabc4ceee1480d885380a59c37`  
		Last Modified: Thu, 17 Sep 2020 01:14:32 GMT  
		Size: 82.5 MB (82512002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aee0e8778e20d8f3114bcaeceb4c0dd4d54a495665f21d495fa9f2bc956d69`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694594587433345707b0eb20693bae9924990a034bb41551ff32a25732dfae0c`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.24-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f6866f9b8c5c04bab5299827002b624a2b330010ce0fe1a3b9048d593068c87a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116815031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d7c574ae73596b744870667c1144f4d0b224c49ed45494fa679c3768a288b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:33:37 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 17 Sep 2020 00:33:38 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Thu, 17 Sep 2020 00:33:40 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:34:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:34:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:34:30 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:34:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:34:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:34:35 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:34:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2c304b19aabdb5b2d97c6cf9387086880a09dc307a28c01de5e729981b327`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1b7e546454a80634c5c004e80de39c5384331b724a6252a898710dfe070624`  
		Last Modified: Thu, 17 Sep 2020 00:39:50 GMT  
		Size: 81.7 MB (81663466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1369725b701991b582b2c14f6a8e4f46bcf1e2d2b0d34901ac164e4699a2f82c`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e071e3d1b3531c578027ef9c0140972c7112306c6c7c6cfbbb3ee36547bf1a05`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3.24-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6ada9a72057b09698f940a19061ed21345c69de1638caf1ae7f6aebea55fd946
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129011810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be004206f8c63f53a64ff60d2bde11541c889278fa4d861eb4aee77718335d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:20:11 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 19 Aug 2020 23:20:23 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Wed, 19 Aug 2020 23:20:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:28:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:28:25 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:28:29 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:28:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:28:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:28:46 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:28:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f324cbd967ceab87e63252c88e75d723fe929ad23856787ac94973461a1f3499`  
		Last Modified: Wed, 19 Aug 2020 23:49:51 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daaecc0bb5f0b8aa41068b03046d09dd4b04aea298f52bc01fb614f78cb4a3d`  
		Last Modified: Wed, 19 Aug 2020 23:50:10 GMT  
		Size: 86.5 MB (86503749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240555122f3825796c16c25757b030eb667ffe353b470e0557462564512a17e9`  
		Last Modified: Wed, 19 Aug 2020 23:49:53 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea38786ce8caadcec478b7302a1bf2c2580eb82c1b40b17c1601c0f778b4a2`  
		Last Modified: Wed, 19 Aug 2020 23:49:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.3-focal`

```console
$ docker pull mariadb@sha256:bf94a1e968e256b0c8b13be4e2ce8f02266dd514361b31de5484734ee6b367d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.3-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:07988d63348d04e66e3b78422ed0d47f561a59ebb38620fe25cb08241755a141
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119157984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16f787686dec1308849e08dd22202f038982cd934ba624f7a1b4b81d1c00bb75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:10:17 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 17 Sep 2020 01:10:17 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Thu, 17 Sep 2020 01:10:18 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:10:57 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:10:58 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:10:58 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:10:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:10:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:10:59 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:10:59 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420ae5e12220ef79c1f0cef0a708cb1b8ad217f4e595290a9aee6ebbb9943224`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7539ff915a5c293690d5f1321a7f729747c28beabc4ceee1480d885380a59c37`  
		Last Modified: Thu, 17 Sep 2020 01:14:32 GMT  
		Size: 82.5 MB (82512002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45aee0e8778e20d8f3114bcaeceb4c0dd4d54a495665f21d495fa9f2bc956d69`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694594587433345707b0eb20693bae9924990a034bb41551ff32a25732dfae0c`  
		Last Modified: Thu, 17 Sep 2020 01:14:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:f6866f9b8c5c04bab5299827002b624a2b330010ce0fe1a3b9048d593068c87a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.8 MB (116815031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82d7c574ae73596b744870667c1144f4d0b224c49ed45494fa679c3768a288b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:33:37 GMT
ENV MARIADB_MAJOR=10.3
# Thu, 17 Sep 2020 00:33:38 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Thu, 17 Sep 2020 00:33:40 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:34:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:34:29 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:34:30 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:34:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:34:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:34:35 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:34:36 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb2c304b19aabdb5b2d97c6cf9387086880a09dc307a28c01de5e729981b327`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1b7e546454a80634c5c004e80de39c5384331b724a6252a898710dfe070624`  
		Last Modified: Thu, 17 Sep 2020 00:39:50 GMT  
		Size: 81.7 MB (81663466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1369725b701991b582b2c14f6a8e4f46bcf1e2d2b0d34901ac164e4699a2f82c`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e071e3d1b3531c578027ef9c0140972c7112306c6c7c6cfbbb3ee36547bf1a05`  
		Last Modified: Thu, 17 Sep 2020 00:39:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.3-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:6ada9a72057b09698f940a19061ed21345c69de1638caf1ae7f6aebea55fd946
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129011810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be004206f8c63f53a64ff60d2bde11541c889278fa4d861eb4aee77718335d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:20:11 GMT
ENV MARIADB_MAJOR=10.3
# Wed, 19 Aug 2020 23:20:23 GMT
ENV MARIADB_VERSION=1:10.3.24+maria~focal
# Wed, 19 Aug 2020 23:20:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:28:14 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:28:25 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:28:29 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:28:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:28:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:28:46 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:28:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f324cbd967ceab87e63252c88e75d723fe929ad23856787ac94973461a1f3499`  
		Last Modified: Wed, 19 Aug 2020 23:49:51 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daaecc0bb5f0b8aa41068b03046d09dd4b04aea298f52bc01fb614f78cb4a3d`  
		Last Modified: Wed, 19 Aug 2020 23:50:10 GMT  
		Size: 86.5 MB (86503749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240555122f3825796c16c25757b030eb667ffe353b470e0557462564512a17e9`  
		Last Modified: Wed, 19 Aug 2020 23:49:53 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea38786ce8caadcec478b7302a1bf2c2580eb82c1b40b17c1601c0f778b4a2`  
		Last Modified: Wed, 19 Aug 2020 23:49:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4`

```console
$ docker pull mariadb@sha256:165930339a6282468328563afc06cd9acb46bcbf165f916c3e18d39bc7deb46f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4` - linux; amd64

```console
$ docker pull mariadb@sha256:ef5e13f094bec3b1bff783f489f91a018db508add163ba05536020b578c86f6b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123515332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:582447dd222436d884a22267bfa73745979b23305f4b5f3dc4a5beef84e2f34b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:09:37 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 17 Sep 2020 01:09:37 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Thu, 17 Sep 2020 01:09:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:10:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:10:11 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:10:11 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:10:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:10:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:10:13 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:10:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e052b281ad7ef1594b765f32039154f2b196e48ca588b87ea62e41b0d6262f`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf994931cc1c77f20dd095c3e724b7bb77b372f92849d5e3cc728b87eb417cf`  
		Last Modified: Thu, 17 Sep 2020 01:14:11 GMT  
		Size: 86.9 MB (86869352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5480c6ee0b2ba3bfd13f1a9746500a38ee2ea7396a22b6fb048c58f209e512`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb19a0bf200da6d492ca1567ad2b85ae9c680f03d39d116dc7061195c79346`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e3f226476e2af1cc2acc0f236ac45b12015a5cf3872c096edc98179f5449f9ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121146361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e0264550074523a77787de20c8b4b39667149fb42e702cfb7f2cb3f37cfe17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:32:40 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 17 Sep 2020 00:32:40 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Thu, 17 Sep 2020 00:32:42 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:33:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:33:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:33:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:33:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:33:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:33:28 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:33:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c28d156edd9beeb816bda91b512e0ffe2fc062d6eab08ca00a7ba0d94471ff`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996792613a2079192fd715a0b64443d4437fdd542b64fce34e472ffb0a4d433f`  
		Last Modified: Thu, 17 Sep 2020 00:39:17 GMT  
		Size: 86.0 MB (85994798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae7988a6f2a08ab84d230289ca3c7fc4a69b88a94d4e8f74b81b414037d9b33`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 5.1 KB (5055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f20b910bf5f4494386216b5a32afb3940b2151635df41ce45b030828f5ff38`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4` - linux; ppc64le

```console
$ docker pull mariadb@sha256:46196b8931eba33168ef15ae8f43cca28c80cd106a5a3fcf1695ac2d7dfcc599
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133520333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a93b7ffe80f449d6036540a1cf74194413fe2220844eeaeb34b99272261962c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:12:42 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 19 Aug 2020 23:12:47 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Wed, 19 Aug 2020 23:12:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:19:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:19:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:19:21 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:19:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:19:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:19:47 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:19:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8565334d4b019c1d27b9f18b03e078fbc145dd350178c3d3a66b01a24a8fe4b5`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8450ab343eb1b9ad3f9e5ee65e3da2a18fccb25c9326ad57a36c997611520ba8`  
		Last Modified: Wed, 19 Aug 2020 23:49:34 GMT  
		Size: 91.0 MB (91012275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462d93d00393368e98cab028e4f524d95f519ecb6686775743230a36b0339fbc`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83827f9e90f2cc0aa7fbda8032957d686af51976cc461e07b10667e983be894e`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.14`

```console
$ docker pull mariadb@sha256:165930339a6282468328563afc06cd9acb46bcbf165f916c3e18d39bc7deb46f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.14` - linux; amd64

```console
$ docker pull mariadb@sha256:ef5e13f094bec3b1bff783f489f91a018db508add163ba05536020b578c86f6b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123515332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:582447dd222436d884a22267bfa73745979b23305f4b5f3dc4a5beef84e2f34b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:09:37 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 17 Sep 2020 01:09:37 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Thu, 17 Sep 2020 01:09:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:10:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:10:11 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:10:11 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:10:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:10:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:10:13 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:10:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e052b281ad7ef1594b765f32039154f2b196e48ca588b87ea62e41b0d6262f`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf994931cc1c77f20dd095c3e724b7bb77b372f92849d5e3cc728b87eb417cf`  
		Last Modified: Thu, 17 Sep 2020 01:14:11 GMT  
		Size: 86.9 MB (86869352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5480c6ee0b2ba3bfd13f1a9746500a38ee2ea7396a22b6fb048c58f209e512`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb19a0bf200da6d492ca1567ad2b85ae9c680f03d39d116dc7061195c79346`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.14` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e3f226476e2af1cc2acc0f236ac45b12015a5cf3872c096edc98179f5449f9ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121146361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e0264550074523a77787de20c8b4b39667149fb42e702cfb7f2cb3f37cfe17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:32:40 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 17 Sep 2020 00:32:40 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Thu, 17 Sep 2020 00:32:42 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:33:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:33:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:33:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:33:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:33:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:33:28 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:33:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c28d156edd9beeb816bda91b512e0ffe2fc062d6eab08ca00a7ba0d94471ff`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996792613a2079192fd715a0b64443d4437fdd542b64fce34e472ffb0a4d433f`  
		Last Modified: Thu, 17 Sep 2020 00:39:17 GMT  
		Size: 86.0 MB (85994798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae7988a6f2a08ab84d230289ca3c7fc4a69b88a94d4e8f74b81b414037d9b33`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 5.1 KB (5055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f20b910bf5f4494386216b5a32afb3940b2151635df41ce45b030828f5ff38`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.14` - linux; ppc64le

```console
$ docker pull mariadb@sha256:46196b8931eba33168ef15ae8f43cca28c80cd106a5a3fcf1695ac2d7dfcc599
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133520333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a93b7ffe80f449d6036540a1cf74194413fe2220844eeaeb34b99272261962c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:12:42 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 19 Aug 2020 23:12:47 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Wed, 19 Aug 2020 23:12:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:19:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:19:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:19:21 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:19:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:19:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:19:47 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:19:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8565334d4b019c1d27b9f18b03e078fbc145dd350178c3d3a66b01a24a8fe4b5`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8450ab343eb1b9ad3f9e5ee65e3da2a18fccb25c9326ad57a36c997611520ba8`  
		Last Modified: Wed, 19 Aug 2020 23:49:34 GMT  
		Size: 91.0 MB (91012275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462d93d00393368e98cab028e4f524d95f519ecb6686775743230a36b0339fbc`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83827f9e90f2cc0aa7fbda8032957d686af51976cc461e07b10667e983be894e`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4.14-focal`

```console
$ docker pull mariadb@sha256:165930339a6282468328563afc06cd9acb46bcbf165f916c3e18d39bc7deb46f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4.14-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:ef5e13f094bec3b1bff783f489f91a018db508add163ba05536020b578c86f6b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123515332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:582447dd222436d884a22267bfa73745979b23305f4b5f3dc4a5beef84e2f34b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:09:37 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 17 Sep 2020 01:09:37 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Thu, 17 Sep 2020 01:09:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:10:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:10:11 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:10:11 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:10:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:10:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:10:13 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:10:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e052b281ad7ef1594b765f32039154f2b196e48ca588b87ea62e41b0d6262f`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf994931cc1c77f20dd095c3e724b7bb77b372f92849d5e3cc728b87eb417cf`  
		Last Modified: Thu, 17 Sep 2020 01:14:11 GMT  
		Size: 86.9 MB (86869352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5480c6ee0b2ba3bfd13f1a9746500a38ee2ea7396a22b6fb048c58f209e512`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb19a0bf200da6d492ca1567ad2b85ae9c680f03d39d116dc7061195c79346`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.14-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e3f226476e2af1cc2acc0f236ac45b12015a5cf3872c096edc98179f5449f9ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121146361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e0264550074523a77787de20c8b4b39667149fb42e702cfb7f2cb3f37cfe17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:32:40 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 17 Sep 2020 00:32:40 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Thu, 17 Sep 2020 00:32:42 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:33:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:33:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:33:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:33:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:33:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:33:28 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:33:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c28d156edd9beeb816bda91b512e0ffe2fc062d6eab08ca00a7ba0d94471ff`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996792613a2079192fd715a0b64443d4437fdd542b64fce34e472ffb0a4d433f`  
		Last Modified: Thu, 17 Sep 2020 00:39:17 GMT  
		Size: 86.0 MB (85994798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae7988a6f2a08ab84d230289ca3c7fc4a69b88a94d4e8f74b81b414037d9b33`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 5.1 KB (5055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f20b910bf5f4494386216b5a32afb3940b2151635df41ce45b030828f5ff38`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4.14-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:46196b8931eba33168ef15ae8f43cca28c80cd106a5a3fcf1695ac2d7dfcc599
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133520333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a93b7ffe80f449d6036540a1cf74194413fe2220844eeaeb34b99272261962c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:12:42 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 19 Aug 2020 23:12:47 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Wed, 19 Aug 2020 23:12:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:19:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:19:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:19:21 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:19:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:19:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:19:47 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:19:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8565334d4b019c1d27b9f18b03e078fbc145dd350178c3d3a66b01a24a8fe4b5`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8450ab343eb1b9ad3f9e5ee65e3da2a18fccb25c9326ad57a36c997611520ba8`  
		Last Modified: Wed, 19 Aug 2020 23:49:34 GMT  
		Size: 91.0 MB (91012275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462d93d00393368e98cab028e4f524d95f519ecb6686775743230a36b0339fbc`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83827f9e90f2cc0aa7fbda8032957d686af51976cc461e07b10667e983be894e`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.4-focal`

```console
$ docker pull mariadb@sha256:165930339a6282468328563afc06cd9acb46bcbf165f916c3e18d39bc7deb46f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.4-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:ef5e13f094bec3b1bff783f489f91a018db508add163ba05536020b578c86f6b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123515332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:582447dd222436d884a22267bfa73745979b23305f4b5f3dc4a5beef84e2f34b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:09:37 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 17 Sep 2020 01:09:37 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Thu, 17 Sep 2020 01:09:38 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:10:11 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:10:11 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:10:11 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:10:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 01:10:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:10:13 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:10:13 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e052b281ad7ef1594b765f32039154f2b196e48ca588b87ea62e41b0d6262f`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf994931cc1c77f20dd095c3e724b7bb77b372f92849d5e3cc728b87eb417cf`  
		Last Modified: Thu, 17 Sep 2020 01:14:11 GMT  
		Size: 86.9 MB (86869352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5480c6ee0b2ba3bfd13f1a9746500a38ee2ea7396a22b6fb048c58f209e512`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb19a0bf200da6d492ca1567ad2b85ae9c680f03d39d116dc7061195c79346`  
		Last Modified: Thu, 17 Sep 2020 01:13:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:e3f226476e2af1cc2acc0f236ac45b12015a5cf3872c096edc98179f5449f9ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121146361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e0264550074523a77787de20c8b4b39667149fb42e702cfb7f2cb3f37cfe17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:32:40 GMT
ENV MARIADB_MAJOR=10.4
# Thu, 17 Sep 2020 00:32:40 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Thu, 17 Sep 2020 00:32:42 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:33:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:33:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:33:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:33:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 17 Sep 2020 00:33:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:33:28 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:33:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c28d156edd9beeb816bda91b512e0ffe2fc062d6eab08ca00a7ba0d94471ff`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996792613a2079192fd715a0b64443d4437fdd542b64fce34e472ffb0a4d433f`  
		Last Modified: Thu, 17 Sep 2020 00:39:17 GMT  
		Size: 86.0 MB (85994798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae7988a6f2a08ab84d230289ca3c7fc4a69b88a94d4e8f74b81b414037d9b33`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 5.1 KB (5055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f20b910bf5f4494386216b5a32afb3940b2151635df41ce45b030828f5ff38`  
		Last Modified: Thu, 17 Sep 2020 00:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.4-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:46196b8931eba33168ef15ae8f43cca28c80cd106a5a3fcf1695ac2d7dfcc599
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133520333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a93b7ffe80f449d6036540a1cf74194413fe2220844eeaeb34b99272261962c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:12:42 GMT
ENV MARIADB_MAJOR=10.4
# Wed, 19 Aug 2020 23:12:47 GMT
ENV MARIADB_VERSION=1:10.4.14+maria~focal
# Wed, 19 Aug 2020 23:12:55 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:19:06 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:19:17 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:19:21 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:19:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 19 Aug 2020 23:19:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:19:47 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:19:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8565334d4b019c1d27b9f18b03e078fbc145dd350178c3d3a66b01a24a8fe4b5`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8450ab343eb1b9ad3f9e5ee65e3da2a18fccb25c9326ad57a36c997611520ba8`  
		Last Modified: Wed, 19 Aug 2020 23:49:34 GMT  
		Size: 91.0 MB (91012275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462d93d00393368e98cab028e4f524d95f519ecb6686775743230a36b0339fbc`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 5.1 KB (5059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83827f9e90f2cc0aa7fbda8032957d686af51976cc461e07b10667e983be894e`  
		Last Modified: Wed, 19 Aug 2020 23:49:14 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5`

```console
$ docker pull mariadb@sha256:d4138c98d16f605afc697e04e7acc9da49c455441a5f6fc85ac97e758eddc6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5` - linux; amd64

```console
$ docker pull mariadb@sha256:49c69c49cd3a725dba2e2687efc573160b16ec841c00c8a14858833050538bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125548061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff8572fa8c9edd0d2f88f03f4dc6d0e6e0c6b03be8e97bae4efd8ba76f45f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 01:08:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:09:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:09:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:09:26 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:09:27 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:09:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0222c6c4a45266f80f02da181a859e16c1746abe2cd1efda692ee4c9fa8a92a5`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab34d00af2f2502f1a8fd16103bf01ac430298666bfdfea989d8a2ac5193cf6`  
		Last Modified: Thu, 17 Sep 2020 01:13:45 GMT  
		Size: 88.9 MB (88902202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb48a5d6fdc6e4e1d8b91b2f30d10947db49be0ce584162fdead9de45bd909ba`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ffb01b700175307f942c997707101d39b938faf6b93ce97fbf17cbb7a0b06d66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123199206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89c7551a9f203b5bee56c2843a7ea98e5c34f6c5a8fab93cab697e5d55d04d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:31:43 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 00:31:44 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 00:31:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:32:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:32:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:32:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:32:26 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:32:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a96525514d40a4b5fa80950555be20f4aacb9a9271898d6ccccea5249badb`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fadbb2548d657860f32dc7d8c389fed772825c82c0d1d3b8bd7a376dbf414e`  
		Last Modified: Thu, 17 Sep 2020 00:38:35 GMT  
		Size: 88.0 MB (88047764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b2f72fd388ebb0795799efcfaff3b3c81b5e91e5fbde3cb56c24e9162efc2`  
		Last Modified: Thu, 17 Sep 2020 00:38:09 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8e30af10e119a02913a96b7d011c49f4c8e0bf868b93abae93b42c0f7a9c92ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135633547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b12d26459ccb7e6a7cbd83d66d721c98a144f18f44f189b21cc3993df05caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:05:24 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 19 Aug 2020 23:05:31 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Wed, 19 Aug 2020 23:05:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:12:01 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:12:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:12:12 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:12:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:12:18 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:12:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3de7a14dd93d9c85fd1768b2474e3bac42e73a9413a78be18d119cd2b3699d`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cebafb1fc8f371df5ff85fe7ed5667891f1c279eb78fdf0ff64635b9e53d36`  
		Last Modified: Wed, 19 Aug 2020 23:48:45 GMT  
		Size: 93.1 MB (93125609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88dba223ea3336bf9cbf0ca0c208c5e98a71b6eba6046ba8adad48a3168a7b3`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 5.1 KB (5060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.5`

```console
$ docker pull mariadb@sha256:d4138c98d16f605afc697e04e7acc9da49c455441a5f6fc85ac97e758eddc6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.5` - linux; amd64

```console
$ docker pull mariadb@sha256:49c69c49cd3a725dba2e2687efc573160b16ec841c00c8a14858833050538bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125548061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff8572fa8c9edd0d2f88f03f4dc6d0e6e0c6b03be8e97bae4efd8ba76f45f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 01:08:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:09:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:09:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:09:26 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:09:27 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:09:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0222c6c4a45266f80f02da181a859e16c1746abe2cd1efda692ee4c9fa8a92a5`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab34d00af2f2502f1a8fd16103bf01ac430298666bfdfea989d8a2ac5193cf6`  
		Last Modified: Thu, 17 Sep 2020 01:13:45 GMT  
		Size: 88.9 MB (88902202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb48a5d6fdc6e4e1d8b91b2f30d10947db49be0ce584162fdead9de45bd909ba`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.5` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ffb01b700175307f942c997707101d39b938faf6b93ce97fbf17cbb7a0b06d66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123199206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89c7551a9f203b5bee56c2843a7ea98e5c34f6c5a8fab93cab697e5d55d04d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:31:43 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 00:31:44 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 00:31:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:32:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:32:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:32:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:32:26 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:32:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a96525514d40a4b5fa80950555be20f4aacb9a9271898d6ccccea5249badb`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fadbb2548d657860f32dc7d8c389fed772825c82c0d1d3b8bd7a376dbf414e`  
		Last Modified: Thu, 17 Sep 2020 00:38:35 GMT  
		Size: 88.0 MB (88047764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b2f72fd388ebb0795799efcfaff3b3c81b5e91e5fbde3cb56c24e9162efc2`  
		Last Modified: Thu, 17 Sep 2020 00:38:09 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.5` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8e30af10e119a02913a96b7d011c49f4c8e0bf868b93abae93b42c0f7a9c92ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135633547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b12d26459ccb7e6a7cbd83d66d721c98a144f18f44f189b21cc3993df05caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:05:24 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 19 Aug 2020 23:05:31 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Wed, 19 Aug 2020 23:05:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:12:01 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:12:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:12:12 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:12:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:12:18 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:12:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3de7a14dd93d9c85fd1768b2474e3bac42e73a9413a78be18d119cd2b3699d`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cebafb1fc8f371df5ff85fe7ed5667891f1c279eb78fdf0ff64635b9e53d36`  
		Last Modified: Wed, 19 Aug 2020 23:48:45 GMT  
		Size: 93.1 MB (93125609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88dba223ea3336bf9cbf0ca0c208c5e98a71b6eba6046ba8adad48a3168a7b3`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 5.1 KB (5060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5.5-focal`

```console
$ docker pull mariadb@sha256:d4138c98d16f605afc697e04e7acc9da49c455441a5f6fc85ac97e758eddc6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:49c69c49cd3a725dba2e2687efc573160b16ec841c00c8a14858833050538bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125548061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff8572fa8c9edd0d2f88f03f4dc6d0e6e0c6b03be8e97bae4efd8ba76f45f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 01:08:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:09:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:09:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:09:26 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:09:27 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:09:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0222c6c4a45266f80f02da181a859e16c1746abe2cd1efda692ee4c9fa8a92a5`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab34d00af2f2502f1a8fd16103bf01ac430298666bfdfea989d8a2ac5193cf6`  
		Last Modified: Thu, 17 Sep 2020 01:13:45 GMT  
		Size: 88.9 MB (88902202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb48a5d6fdc6e4e1d8b91b2f30d10947db49be0ce584162fdead9de45bd909ba`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ffb01b700175307f942c997707101d39b938faf6b93ce97fbf17cbb7a0b06d66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123199206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89c7551a9f203b5bee56c2843a7ea98e5c34f6c5a8fab93cab697e5d55d04d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:31:43 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 00:31:44 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 00:31:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:32:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:32:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:32:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:32:26 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:32:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a96525514d40a4b5fa80950555be20f4aacb9a9271898d6ccccea5249badb`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fadbb2548d657860f32dc7d8c389fed772825c82c0d1d3b8bd7a376dbf414e`  
		Last Modified: Thu, 17 Sep 2020 00:38:35 GMT  
		Size: 88.0 MB (88047764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b2f72fd388ebb0795799efcfaff3b3c81b5e91e5fbde3cb56c24e9162efc2`  
		Last Modified: Thu, 17 Sep 2020 00:38:09 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8e30af10e119a02913a96b7d011c49f4c8e0bf868b93abae93b42c0f7a9c92ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135633547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b12d26459ccb7e6a7cbd83d66d721c98a144f18f44f189b21cc3993df05caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:05:24 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 19 Aug 2020 23:05:31 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Wed, 19 Aug 2020 23:05:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:12:01 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:12:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:12:12 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:12:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:12:18 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:12:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3de7a14dd93d9c85fd1768b2474e3bac42e73a9413a78be18d119cd2b3699d`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cebafb1fc8f371df5ff85fe7ed5667891f1c279eb78fdf0ff64635b9e53d36`  
		Last Modified: Wed, 19 Aug 2020 23:48:45 GMT  
		Size: 93.1 MB (93125609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88dba223ea3336bf9cbf0ca0c208c5e98a71b6eba6046ba8adad48a3168a7b3`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 5.1 KB (5060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10.5-focal`

```console
$ docker pull mariadb@sha256:d4138c98d16f605afc697e04e7acc9da49c455441a5f6fc85ac97e758eddc6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10.5-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:49c69c49cd3a725dba2e2687efc573160b16ec841c00c8a14858833050538bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125548061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff8572fa8c9edd0d2f88f03f4dc6d0e6e0c6b03be8e97bae4efd8ba76f45f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 01:08:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:09:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:09:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:09:26 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:09:27 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:09:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0222c6c4a45266f80f02da181a859e16c1746abe2cd1efda692ee4c9fa8a92a5`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab34d00af2f2502f1a8fd16103bf01ac430298666bfdfea989d8a2ac5193cf6`  
		Last Modified: Thu, 17 Sep 2020 01:13:45 GMT  
		Size: 88.9 MB (88902202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb48a5d6fdc6e4e1d8b91b2f30d10947db49be0ce584162fdead9de45bd909ba`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ffb01b700175307f942c997707101d39b938faf6b93ce97fbf17cbb7a0b06d66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123199206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89c7551a9f203b5bee56c2843a7ea98e5c34f6c5a8fab93cab697e5d55d04d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:31:43 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 00:31:44 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 00:31:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:32:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:32:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:32:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:32:26 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:32:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a96525514d40a4b5fa80950555be20f4aacb9a9271898d6ccccea5249badb`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fadbb2548d657860f32dc7d8c389fed772825c82c0d1d3b8bd7a376dbf414e`  
		Last Modified: Thu, 17 Sep 2020 00:38:35 GMT  
		Size: 88.0 MB (88047764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b2f72fd388ebb0795799efcfaff3b3c81b5e91e5fbde3cb56c24e9162efc2`  
		Last Modified: Thu, 17 Sep 2020 00:38:09 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10.5-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8e30af10e119a02913a96b7d011c49f4c8e0bf868b93abae93b42c0f7a9c92ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135633547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b12d26459ccb7e6a7cbd83d66d721c98a144f18f44f189b21cc3993df05caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:05:24 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 19 Aug 2020 23:05:31 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Wed, 19 Aug 2020 23:05:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:12:01 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:12:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:12:12 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:12:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:12:18 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:12:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3de7a14dd93d9c85fd1768b2474e3bac42e73a9413a78be18d119cd2b3699d`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cebafb1fc8f371df5ff85fe7ed5667891f1c279eb78fdf0ff64635b9e53d36`  
		Last Modified: Wed, 19 Aug 2020 23:48:45 GMT  
		Size: 93.1 MB (93125609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88dba223ea3336bf9cbf0ca0c208c5e98a71b6eba6046ba8adad48a3168a7b3`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 5.1 KB (5060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:10-focal`

```console
$ docker pull mariadb@sha256:d4138c98d16f605afc697e04e7acc9da49c455441a5f6fc85ac97e758eddc6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:10-focal` - linux; amd64

```console
$ docker pull mariadb@sha256:49c69c49cd3a725dba2e2687efc573160b16ec841c00c8a14858833050538bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125548061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff8572fa8c9edd0d2f88f03f4dc6d0e6e0c6b03be8e97bae4efd8ba76f45f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 01:08:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:09:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:09:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:09:26 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:09:27 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:09:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0222c6c4a45266f80f02da181a859e16c1746abe2cd1efda692ee4c9fa8a92a5`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab34d00af2f2502f1a8fd16103bf01ac430298666bfdfea989d8a2ac5193cf6`  
		Last Modified: Thu, 17 Sep 2020 01:13:45 GMT  
		Size: 88.9 MB (88902202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb48a5d6fdc6e4e1d8b91b2f30d10947db49be0ce584162fdead9de45bd909ba`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ffb01b700175307f942c997707101d39b938faf6b93ce97fbf17cbb7a0b06d66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123199206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89c7551a9f203b5bee56c2843a7ea98e5c34f6c5a8fab93cab697e5d55d04d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:31:43 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 00:31:44 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 00:31:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:32:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:32:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:32:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:32:26 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:32:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a96525514d40a4b5fa80950555be20f4aacb9a9271898d6ccccea5249badb`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fadbb2548d657860f32dc7d8c389fed772825c82c0d1d3b8bd7a376dbf414e`  
		Last Modified: Thu, 17 Sep 2020 00:38:35 GMT  
		Size: 88.0 MB (88047764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b2f72fd388ebb0795799efcfaff3b3c81b5e91e5fbde3cb56c24e9162efc2`  
		Last Modified: Thu, 17 Sep 2020 00:38:09 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:10-focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8e30af10e119a02913a96b7d011c49f4c8e0bf868b93abae93b42c0f7a9c92ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135633547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b12d26459ccb7e6a7cbd83d66d721c98a144f18f44f189b21cc3993df05caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:05:24 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 19 Aug 2020 23:05:31 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Wed, 19 Aug 2020 23:05:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:12:01 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:12:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:12:12 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:12:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:12:18 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:12:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3de7a14dd93d9c85fd1768b2474e3bac42e73a9413a78be18d119cd2b3699d`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cebafb1fc8f371df5ff85fe7ed5667891f1c279eb78fdf0ff64635b9e53d36`  
		Last Modified: Wed, 19 Aug 2020 23:48:45 GMT  
		Size: 93.1 MB (93125609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88dba223ea3336bf9cbf0ca0c208c5e98a71b6eba6046ba8adad48a3168a7b3`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 5.1 KB (5060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:focal`

```console
$ docker pull mariadb@sha256:d4138c98d16f605afc697e04e7acc9da49c455441a5f6fc85ac97e758eddc6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:focal` - linux; amd64

```console
$ docker pull mariadb@sha256:49c69c49cd3a725dba2e2687efc573160b16ec841c00c8a14858833050538bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125548061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff8572fa8c9edd0d2f88f03f4dc6d0e6e0c6b03be8e97bae4efd8ba76f45f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 01:08:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:09:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:09:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:09:26 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:09:27 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:09:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0222c6c4a45266f80f02da181a859e16c1746abe2cd1efda692ee4c9fa8a92a5`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab34d00af2f2502f1a8fd16103bf01ac430298666bfdfea989d8a2ac5193cf6`  
		Last Modified: Thu, 17 Sep 2020 01:13:45 GMT  
		Size: 88.9 MB (88902202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb48a5d6fdc6e4e1d8b91b2f30d10947db49be0ce584162fdead9de45bd909ba`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ffb01b700175307f942c997707101d39b938faf6b93ce97fbf17cbb7a0b06d66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123199206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89c7551a9f203b5bee56c2843a7ea98e5c34f6c5a8fab93cab697e5d55d04d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:31:43 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 00:31:44 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 00:31:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:32:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:32:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:32:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:32:26 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:32:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a96525514d40a4b5fa80950555be20f4aacb9a9271898d6ccccea5249badb`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fadbb2548d657860f32dc7d8c389fed772825c82c0d1d3b8bd7a376dbf414e`  
		Last Modified: Thu, 17 Sep 2020 00:38:35 GMT  
		Size: 88.0 MB (88047764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b2f72fd388ebb0795799efcfaff3b3c81b5e91e5fbde3cb56c24e9162efc2`  
		Last Modified: Thu, 17 Sep 2020 00:38:09 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:focal` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8e30af10e119a02913a96b7d011c49f4c8e0bf868b93abae93b42c0f7a9c92ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135633547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b12d26459ccb7e6a7cbd83d66d721c98a144f18f44f189b21cc3993df05caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:05:24 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 19 Aug 2020 23:05:31 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Wed, 19 Aug 2020 23:05:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:12:01 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:12:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:12:12 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:12:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:12:18 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:12:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3de7a14dd93d9c85fd1768b2474e3bac42e73a9413a78be18d119cd2b3699d`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cebafb1fc8f371df5ff85fe7ed5667891f1c279eb78fdf0ff64635b9e53d36`  
		Last Modified: Wed, 19 Aug 2020 23:48:45 GMT  
		Size: 93.1 MB (93125609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88dba223ea3336bf9cbf0ca0c208c5e98a71b6eba6046ba8adad48a3168a7b3`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 5.1 KB (5060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mariadb:latest`

```console
$ docker pull mariadb@sha256:d4138c98d16f605afc697e04e7acc9da49c455441a5f6fc85ac97e758eddc6da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `mariadb:latest` - linux; amd64

```console
$ docker pull mariadb@sha256:49c69c49cd3a725dba2e2687efc573160b16ec841c00c8a14858833050538bdb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125548061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbbff8572fa8c9edd0d2f88f03f4dc6d0e6e0c6b03be8e97bae4efd8ba76f45f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 22:20:23 GMT
ADD file:1b4ec50586b9f0621095f51ee6baecc00a7f6d95b4a04e3bedc5393b28bc8a54 in / 
# Wed, 16 Sep 2020 22:20:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:20:24 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 22:20:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:20:25 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 01:08:33 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 01:08:41 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:41 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 01:08:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 01:08:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 01:08:57 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 01:08:58 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 01:08:58 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 01:08:59 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 01:09:26 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 01:09:26 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 01:09:26 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 01:09:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 01:09:27 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 01:09:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e6ca3592b14484be6a9719617680e0c810e0107d89c437162c75d2401637c72c`  
		Last Modified: Wed, 16 Sep 2020 15:19:59 GMT  
		Size: 28.6 MB (28557166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534a5505201da9ddb334b5b2fcb3cec45fcafccd8e91b93ad4852e1a1bb318c1`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 839.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990916bd23bbbf9c30d202dad557e813562d028f3076bf57904830c69d4cde83`  
		Last Modified: Wed, 16 Sep 2020 22:23:09 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62d6bd206a2945755de125028a91e37adf810f67a028c6f36b3617f5f6d8ea0`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba34deb445c3894c6d38a0f50a1944646fe5c5d31e00b9b1826576efcda08578`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 5.5 MB (5488311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b4f6570cf0c052c75c91fc0f0d091de2645ad0687dca9b6e67d7a84d2dda01`  
		Last Modified: Thu, 17 Sep 2020 01:13:29 GMT  
		Size: 1.3 MB (1323902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b039c5139eb47fe9cc8d1eb576d029c54dc902a11ed8be3c014860ace41e0a`  
		Last Modified: Thu, 17 Sep 2020 01:13:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0e67eb23f7d6361faad6376374e1bd786d4d35ef95fcf13fd5ebc3dfc1378`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 1.3 MB (1265755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69df87d9330c3e008224000aa28db2c78323f411bb35b82d0eb2499a1850e924`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0222c6c4a45266f80f02da181a859e16c1746abe2cd1efda692ee4c9fa8a92a5`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab34d00af2f2502f1a8fd16103bf01ac430298666bfdfea989d8a2ac5193cf6`  
		Last Modified: Thu, 17 Sep 2020 01:13:45 GMT  
		Size: 88.9 MB (88902202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb48a5d6fdc6e4e1d8b91b2f30d10947db49be0ce584162fdead9de45bd909ba`  
		Last Modified: Thu, 17 Sep 2020 01:13:27 GMT  
		Size: 5.1 KB (5057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:ffb01b700175307f942c997707101d39b938faf6b93ce97fbf17cbb7a0b06d66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.2 MB (123199206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89c7551a9f203b5bee56c2843a7ea98e5c34f6c5a8fab93cab697e5d55d04d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 16 Sep 2020 23:16:56 GMT
ADD file:063d9d9577619d2eeb19bbc784fecf567039a314d8f741500841f6b4f3c847b3 in / 
# Wed, 16 Sep 2020 23:17:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 23:17:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 16 Sep 2020 23:17:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 23:17:04 GMT
CMD ["/bin/bash"]
# Thu, 17 Sep 2020 00:30:53 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 17 Sep 2020 00:31:10 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:11 GMT
ENV GOSU_VERSION=1.12
# Thu, 17 Sep 2020 00:31:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Sep 2020 00:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Sep 2020 00:31:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Sep 2020 00:31:41 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Thu, 17 Sep 2020 00:31:43 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 17 Sep 2020 00:31:43 GMT
ENV MARIADB_MAJOR=10.5
# Thu, 17 Sep 2020 00:31:44 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Thu, 17 Sep 2020 00:31:46 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Thu, 17 Sep 2020 00:32:22 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Thu, 17 Sep 2020 00:32:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 17 Sep 2020 00:32:25 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Thu, 17 Sep 2020 00:32:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Sep 2020 00:32:26 GMT
EXPOSE 3306
# Thu, 17 Sep 2020 00:32:27 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:33c9bf8777b52e6bc989f3a77a8a680861b9a7f7385e2d5ee02fdede89acf606`  
		Last Modified: Wed, 16 Sep 2020 08:25:33 GMT  
		Size: 27.2 MB (27158462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1900e162114f589f3e78ba5b26957f2b6ec38c8aaa6efdd8afbfaf5d9e8841`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c8a81c25472b52dd428e136c84a1f407ce933911cab5910676d1a7b7a4df3`  
		Last Modified: Wed, 16 Sep 2020 23:18:40 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430efa62b5cb24763fd449fcc3fc98aff5ce773c7a14b9a1be6c1de2eeb85a06`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d211c5ace3f071bbb33d4c6c996d8c6cd0f4a33a05ef8057399bacab1ddef`  
		Last Modified: Thu, 17 Sep 2020 00:38:13 GMT  
		Size: 5.5 MB (5455761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31ef9885cfc4ed7a8098439a6b710ba2ec062cf2a3a9a7f42426987a872c119`  
		Last Modified: Thu, 17 Sep 2020 00:38:12 GMT  
		Size: 1.3 MB (1261149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fb2928c053da58d87d00d26f1808855195a3691a806d868c064b5b9fa148d9`  
		Last Modified: Thu, 17 Sep 2020 00:38:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4644878097ffa32a3fa383322412d96335fce34e94ebb34d72b535d39c2113`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 1.3 MB (1265264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9621a3ac7704230484aa8a4966607fb360a07c87173ef041f5c21c10b7f428d`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a96525514d40a4b5fa80950555be20f4aacb9a9271898d6ccccea5249badb`  
		Last Modified: Thu, 17 Sep 2020 00:38:10 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fadbb2548d657860f32dc7d8c389fed772825c82c0d1d3b8bd7a376dbf414e`  
		Last Modified: Thu, 17 Sep 2020 00:38:35 GMT  
		Size: 88.0 MB (88047764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3b2f72fd388ebb0795799efcfaff3b3c81b5e91e5fbde3cb56c24e9162efc2`  
		Last Modified: Thu, 17 Sep 2020 00:38:09 GMT  
		Size: 5.1 KB (5056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:latest` - linux; ppc64le

```console
$ docker pull mariadb@sha256:8e30af10e119a02913a96b7d011c49f4c8e0bf868b93abae93b42c0f7a9c92ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135633547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5b12d26459ccb7e6a7cbd83d66d721c98a144f18f44f189b21cc3993df05caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:55 GMT
ADD file:505d73c0fde57285890813d908992f8d8f5bdc566faa3371f7b0e69af763548a in / 
# Wed, 19 Aug 2020 21:15:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:15:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:15:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:15:50 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:59:46 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 19 Aug 2020 23:01:09 GMT
RUN set -ex; 	apt-get update; 	if ! which gpg; then 		apt-get install -y --no-install-recommends gnupg; 	fi; 	if ! gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends dirmngr; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:01:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:04:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:05:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		pwgen 		tzdata 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:05:06 GMT
ENV GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Wed, 19 Aug 2020 23:05:19 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mariadb.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:05:24 GMT
ENV MARIADB_MAJOR=10.5
# Wed, 19 Aug 2020 23:05:31 GMT
ENV MARIADB_VERSION=1:10.5.5+maria~focal
# Wed, 19 Aug 2020 23:05:47 GMT
RUN set -e;	echo "deb http://ftp.osuosl.org/pub/mariadb/repo/$MARIADB_MAJOR/ubuntu focal main" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Wed, 19 Aug 2020 23:12:01 GMT
RUN set -ex; 	{ 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password password 'unused'; 		echo "mariadb-server-$MARIADB_MAJOR" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	apt-get install -y 		"mariadb-server=$MARIADB_VERSION" 		mariadb-backup 		socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Wed, 19 Aug 2020 23:12:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 19 Aug 2020 23:12:12 GMT
COPY file:7a2bd14d0848358d403d6a9913bd5da8743de51ba46b60bf676d773828a634a0 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:12:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:12:18 GMT
EXPOSE 3306
# Wed, 19 Aug 2020 23:12:22 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3b0529bc71f72ed0745671e9c10799fcf86fa28062a067d7386f9b1ca76d0f25`  
		Last Modified: Mon, 03 Aug 2020 15:52:06 GMT  
		Size: 33.3 MB (33281555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ffbae55f1eb6509d56c98ef3a98e376eb19f6d8372b400264ade934135312`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 32.2 KB (32167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11405d430f6978a12c2b1c2244fc8605209dba48a4fb192e0bcc76627b0edd32`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fbfc04bfafb23bfaa0c6e20d905d04793fcb9b897f463abda00521e1034e27`  
		Last Modified: Wed, 19 Aug 2020 21:19:09 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eedf35aa7ea75545c8c3909934ff97f7f74ffade1dec19393d5b83628a59fbd`  
		Last Modified: Wed, 19 Aug 2020 23:48:44 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5e64e40d337a4f3f2cefb6cd63cd53b9defb4b3b7cc3e71b2716b4253f3632`  
		Last Modified: Wed, 19 Aug 2020 23:48:41 GMT  
		Size: 6.7 MB (6667707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902303175b2de4cdd27c1a9b72808b714b23b69f3affe95a430079cb6b2a230e`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 1.2 MB (1243039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b738638eadbbcf25ae76677465d8a3603854ee119d1e2ae9f237d3f9132c4a1b`  
		Last Modified: Wed, 19 Aug 2020 23:48:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894d814cc7793b6b2973f5419d8039204eece31da59acf21c85480d9f0e88a79`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 1.3 MB (1272645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c467b7e3d55997c8fa529047e6e1b78a13f76408dff455edc581bb5e6f5db7a`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3de7a14dd93d9c85fd1768b2474e3bac42e73a9413a78be18d119cd2b3699d`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cebafb1fc8f371df5ff85fe7ed5667891f1c279eb78fdf0ff64635b9e53d36`  
		Last Modified: Wed, 19 Aug 2020 23:48:45 GMT  
		Size: 93.1 MB (93125609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88dba223ea3336bf9cbf0ca0c208c5e98a71b6eba6046ba8adad48a3168a7b3`  
		Last Modified: Wed, 19 Aug 2020 23:48:27 GMT  
		Size: 5.1 KB (5060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
