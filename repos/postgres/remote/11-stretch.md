## `postgres:11-stretch`

```console
$ docker pull postgres@sha256:39b264f16d499c57261e39817c67579185d29c64530920c403def1a5632f1d0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:11-stretch` - linux; amd64

```console
$ docker pull postgres@sha256:c95cc2d675299b370ea3f8091ae61ee907abb0c048efe3579e3874acec230ba1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106549299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9707222fa9669553386e5b1139751f2170c88e935708a7d803961f74ed181bea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:30 GMT
ADD file:c7a3b8a1e87bedfb6605855ad703321050112d02c9925ece42f4111d7a42cdd0 in / 
# Tue, 28 Sep 2021 01:25:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 17:30:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 17:30:56 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 17:30:56 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 17:31:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 17:31:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 17:31:16 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 17:31:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 17:31:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 17:31:28 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 17:31:29 GMT
ENV PG_MAJOR=11
# Tue, 28 Sep 2021 17:31:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 28 Sep 2021 17:31:29 GMT
ENV PG_VERSION=11.13-1.pgdg90+1
# Tue, 28 Sep 2021 17:31:59 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 17:32:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 17:32:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 17:32:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 17:32:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 17:32:02 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Sep 2021 17:32:02 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Tue, 28 Sep 2021 17:32:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 17:32:03 GMT
STOPSIGNAL SIGINT
# Tue, 28 Sep 2021 17:32:03 GMT
EXPOSE 5432
# Tue, 28 Sep 2021 17:32:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:36d925ed8e305498a951c3b56d100d153ae3babf046b88e2d00899105fe81c31`  
		Last Modified: Tue, 28 Sep 2021 01:32:51 GMT  
		Size: 22.5 MB (22527699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b0099cd1a09b0b2194a09eade24217dcb33a323b2a9c9fa0b1e9675baef91b`  
		Last Modified: Tue, 28 Sep 2021 17:34:37 GMT  
		Size: 4.5 MB (4503770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf2a548fff24ee8a6e8600d9a56374234c0680c30fa06acac089c9ef8bb098b`  
		Last Modified: Tue, 28 Sep 2021 17:34:36 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6fa05828bd66b1400946230cb0abe47efae886d300472fa79807765aca6f4`  
		Last Modified: Tue, 28 Sep 2021 17:34:36 GMT  
		Size: 1.4 MB (1412200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000ab621c9681911a41670d9e0b8bb0c51a2b35e65521176e331978e6f6d8b4e`  
		Last Modified: Tue, 28 Sep 2021 17:34:35 GMT  
		Size: 6.2 MB (6185581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6855b4b63497ce5eb706ca2d1c07ee4b92780cfb0f81d00277b9196365ed334b`  
		Last Modified: Tue, 28 Sep 2021 17:34:34 GMT  
		Size: 385.0 KB (384996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9201c39bd81382aed94e5f314936bc4ce379b446ffce65b0ae820577eca6157c`  
		Last Modified: Tue, 28 Sep 2021 17:34:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de19e180543b563772c95d696cefc28f3750fa4b9570da276edc631f2078e0a4`  
		Last Modified: Tue, 28 Sep 2021 17:34:33 GMT  
		Size: 5.3 KB (5337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b35f4e5a9332475e330b4de2330357ae974484482d53a33a0cd1c6c21cc394f`  
		Last Modified: Tue, 28 Sep 2021 17:34:42 GMT  
		Size: 71.5 MB (71514696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d401ded3c4b2cfeed7a2af905baee625fada5742ebc578edbb22cdcfa115f4a`  
		Last Modified: Tue, 28 Sep 2021 17:34:31 GMT  
		Size: 8.3 KB (8321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b413e3b3360ea5adaa14f435c0202988ea8fcd6230b3d82bf0df50dbeb952ce2`  
		Last Modified: Tue, 28 Sep 2021 17:34:31 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54896df8d44c1011a466ba384a7ccac8f921adc5b60d575347b2e366b39aa71`  
		Last Modified: Tue, 28 Sep 2021 17:34:31 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44536c25a63655ed00efae3629dc142bf823a0a3dde79c872ff9afad68f0dca`  
		Last Modified: Tue, 28 Sep 2021 17:34:31 GMT  
		Size: 4.4 KB (4409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:ce9a06ee88acf29a38d6cc106c8b7f49144473b98c9c2f0f83e8fea0074a3f98
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70633473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff6c1744a1498a11033aec5dd9a3eb086b0eeb47aed1fb7b4fb491191e95c7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:40 GMT
ADD file:c0e9a99ba405945353742a7ca9ee5f4807d9626de940828c7e91ea7613fbce6b in / 
# Tue, 28 Sep 2021 01:56:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 06:46:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 06:46:02 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 06:46:03 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 06:46:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 06:46:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 06:46:55 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 06:47:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 06:47:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 06:47:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 06:47:21 GMT
ENV PG_MAJOR=11
# Tue, 28 Sep 2021 06:47:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 28 Sep 2021 06:47:22 GMT
ENV PG_VERSION=11.13-1.pgdg90+1
# Tue, 28 Sep 2021 07:13:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 07:13:05 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 07:13:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 07:13:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 07:13:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 07:13:09 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Sep 2021 07:13:09 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Tue, 28 Sep 2021 07:13:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 07:13:10 GMT
STOPSIGNAL SIGINT
# Tue, 28 Sep 2021 07:13:10 GMT
EXPOSE 5432
# Tue, 28 Sep 2021 07:13:11 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bb8e5fcfd7de8c6ce0f02070264ebe0df51ac6b9717272bead263dd7cca70d0b`  
		Last Modified: Tue, 28 Sep 2021 02:14:29 GMT  
		Size: 21.2 MB (21204242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73644ff9757bcb8fb39d6a3b1f344813adfa61e0a5d9c8cdaa2658d0676d6f6c`  
		Last Modified: Tue, 28 Sep 2021 08:57:47 GMT  
		Size: 4.2 MB (4239296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9581d5c8bb5b918c595eb3b441df16f0486030075effd635f73303bf1e93c9`  
		Last Modified: Tue, 28 Sep 2021 08:57:44 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f69dc224794f632860a105721f6276d38a558bcec13ed570c55a9729c87c4e`  
		Last Modified: Tue, 28 Sep 2021 08:57:45 GMT  
		Size: 1.4 MB (1371454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fd2b370b6cd657f3c85a759ccf13677ef00b7105f3045ba9f10de236ee68ae`  
		Last Modified: Tue, 28 Sep 2021 08:57:47 GMT  
		Size: 6.2 MB (6185662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d625d40558540b118f49566d2c79a33e33b747256c90f5c676fd1a5b8b3db9a`  
		Last Modified: Tue, 28 Sep 2021 08:57:43 GMT  
		Size: 385.1 KB (385051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0df4e8a7ddf013a43ab3fed0e023abd64860a2f84de78b531eefd31959823`  
		Last Modified: Tue, 28 Sep 2021 08:57:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d0a12b4a41de11f1ff8d9235398510ca444d8ab81cf1448f27a86d982b020`  
		Last Modified: Tue, 28 Sep 2021 08:57:42 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724109bb60f87892e23bc86dda004cee74a679f7f81c0108c726d1979df2bda0`  
		Last Modified: Tue, 28 Sep 2021 08:58:06 GMT  
		Size: 37.2 MB (37227405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3664f01ff37f8146e77005d01b1140c09fc18751f0c4a79b9ee2864241fe00`  
		Last Modified: Tue, 28 Sep 2021 08:57:41 GMT  
		Size: 8.3 KB (8326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358c27de034006b7559848f1707b63aabc9cdd259cdd5691f1e2b805bc89db63`  
		Last Modified: Tue, 28 Sep 2021 08:57:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23e6890aa1a6df09208a806075d0bceff2dce091872719aa487b229c5a45db4`  
		Last Modified: Tue, 28 Sep 2021 08:57:41 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9068818f9381cc9288d439a06d550b4bab58c15bf2f106c2b6c2471558ac8bb`  
		Last Modified: Tue, 28 Sep 2021 08:57:41 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:9e48bb468c04c669a7720d26c05f13c7971e97180edef673053cf6a792f1ed4c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67299898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67288861827671e11ce386860d4e5ed55368a809bd6217fd423290cd83d479a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 01:05:16 GMT
ADD file:425f8ae3b1354b9858904edb027190b58b65692a710cb50a4d463ac554f853a6 in / 
# Fri, 03 Sep 2021 01:05:17 GMT
CMD ["bash"]
# Sat, 04 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Sep 2021 02:11:04 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 04 Sep 2021 02:11:05 GMT
ENV GOSU_VERSION=1.12
# Sat, 04 Sep 2021 02:11:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 04 Sep 2021 02:11:50 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 04 Sep 2021 02:11:50 GMT
ENV LANG=en_US.utf8
# Sat, 04 Sep 2021 02:11:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:12:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 04 Sep 2021 02:12:13 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 04 Sep 2021 02:12:14 GMT
ENV PG_MAJOR=11
# Sat, 04 Sep 2021 02:12:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sat, 04 Sep 2021 02:12:14 GMT
ENV PG_VERSION=11.13-1.pgdg90+1
# Sat, 04 Sep 2021 02:35:04 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Sep 2021 02:35:06 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Sep 2021 02:35:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Sep 2021 02:35:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Sep 2021 02:35:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Sep 2021 02:35:10 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Sep 2021 02:35:11 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Sat, 04 Sep 2021 02:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:35:12 GMT
STOPSIGNAL SIGINT
# Sat, 04 Sep 2021 02:35:12 GMT
EXPOSE 5432
# Sat, 04 Sep 2021 02:35:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0c15a1a8c9dffe5dfe059b37d14b92f1eb4ea47f16ae7bf66bf62f34a7510dd6`  
		Last Modified: Fri, 03 Sep 2021 01:22:37 GMT  
		Size: 19.3 MB (19316099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642403b1e08021dae4d804216e6501bd8b4a3b34cec478bd4594d6fb139dd9a6`  
		Last Modified: Sat, 04 Sep 2021 04:14:28 GMT  
		Size: 3.9 MB (3875029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa64f67793a8ed73b6ff1146fb4db81a78e28d52ff9ab133ecd2bafc6c88a90e`  
		Last Modified: Sat, 04 Sep 2021 04:14:25 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbcd3ceed3a694d009ad496642ebb964a00f9d7e7760b8cb0c0dc782d374a84`  
		Last Modified: Sat, 04 Sep 2021 04:14:26 GMT  
		Size: 1.4 MB (1363892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f36abad1d80c59106f577f71dd6fb25594c68ee1d5a5a0c4b6dc431276bb93`  
		Last Modified: Sat, 04 Sep 2021 04:14:28 GMT  
		Size: 6.2 MB (6185677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2d438af800bceae74d2bb8c1a7715359edfd08c59d16e2efb6673d08d75f2`  
		Last Modified: Sat, 04 Sep 2021 04:14:24 GMT  
		Size: 379.2 KB (379190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef580edaacbebee4a7089addfbc28818dc888de118bdafc377b80d4d976be0d8`  
		Last Modified: Sat, 04 Sep 2021 04:14:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bd7a8b9c74171813bf055eb26cea24384c3ea40c7a5f122243dba962c80460`  
		Last Modified: Sat, 04 Sep 2021 04:14:23 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a090efad4a1e5f8929e73c11c1f866427e5e5e6f4f65cc30421b31ba3ef67a61`  
		Last Modified: Sat, 04 Sep 2021 04:14:45 GMT  
		Size: 36.2 MB (36159664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667541bf6c0ee2bcbca087a4ba656db9ee41fed5bd5a8eb4db9e66b431ac316b`  
		Last Modified: Sat, 04 Sep 2021 04:14:21 GMT  
		Size: 8.3 KB (8325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cda78481c6cecc9fb54ec242287d9c73e88f831338d072a9dc32982b4b23f3`  
		Last Modified: Sat, 04 Sep 2021 04:14:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6a929d047f2b8ff1fc942d80e2a60b5534ce21ea2dc1650d82fd6d4ed81ce6`  
		Last Modified: Sat, 04 Sep 2021 04:14:21 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e5e69ed342822ad0436f4431ab306e903b02d5bdf9806d9d091053359b660a`  
		Last Modified: Sat, 04 Sep 2021 04:14:21 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:bef549fc7e4ddc268b03a33875205efbb5c9bad1e9f811c735b187f4a42cc37a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69909030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd65098d1c3f21aeae719abdaf39c1202312f6389a60813679aa31d5a6f5e1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:26 GMT
ADD file:be175324382a4d494cf1f644f77b27f17829f187478f9eed602be03b358ffbdc in / 
# Tue, 28 Sep 2021 01:43:27 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 11:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 11:23:40 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 11:23:40 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 11:23:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 11:23:59 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 11:23:59 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 11:24:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 11:24:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 11:24:15 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 11:24:15 GMT
ENV PG_MAJOR=11
# Tue, 28 Sep 2021 11:24:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 28 Sep 2021 11:24:16 GMT
ENV PG_VERSION=11.13-1.pgdg90+1
# Tue, 28 Sep 2021 11:33:40 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 11:33:41 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 11:33:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 11:33:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 11:33:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 11:33:42 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Sep 2021 11:33:42 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Tue, 28 Sep 2021 11:33:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 11:33:43 GMT
STOPSIGNAL SIGINT
# Tue, 28 Sep 2021 11:33:43 GMT
EXPOSE 5432
# Tue, 28 Sep 2021 11:33:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:754614322eeee5db75df451bbdaf75a2049b3ffb0bbcc404a80770f454125583`  
		Last Modified: Tue, 28 Sep 2021 01:52:52 GMT  
		Size: 20.4 MB (20389432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c66dc0f0439952f17ff81d475fd9f303fd7a160a7b1a37f068bc3e3d1d0b02`  
		Last Modified: Tue, 28 Sep 2021 11:58:26 GMT  
		Size: 4.1 MB (4078920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110c52665f42bfc240a88897e37a28a669c3876d39e55fce27d64139aafd2770`  
		Last Modified: Tue, 28 Sep 2021 11:58:25 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b224527b40165c66a822c2b7cb119e61d9e719b23bf8a9cbba1c481cad2cc77e`  
		Last Modified: Tue, 28 Sep 2021 11:58:25 GMT  
		Size: 1.3 MB (1347007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd958bf215af4549f6f9f997f01e7a994e7a84afd160a9fc368cba5ca09f027b`  
		Last Modified: Tue, 28 Sep 2021 11:58:23 GMT  
		Size: 6.2 MB (6185143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dc95d3093c4b910c3d8aaaa6974f2a832161e5cccb60cce75c19b4c52d3407`  
		Last Modified: Tue, 28 Sep 2021 11:58:23 GMT  
		Size: 377.9 KB (377852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc73d8c3095228b0f0825a32dda1b173c25a2b78d086cf3d672436ffe5f5c5cd`  
		Last Modified: Tue, 28 Sep 2021 11:58:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a20fc9638f39345ff08af30613d61a26fe26efd0ebec0801c19ef15c6fcb91`  
		Last Modified: Tue, 28 Sep 2021 11:58:22 GMT  
		Size: 5.3 KB (5339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b8d4dc1d08906f3fb326b5200c417f540eea3af8c7df1076c7688805d8ec55`  
		Last Modified: Tue, 28 Sep 2021 11:58:27 GMT  
		Size: 37.5 MB (37510309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dccec47f37f417f6d8acf1d0c9290d3c456429f5f967166a4615e6ce1d9e6d`  
		Last Modified: Tue, 28 Sep 2021 11:58:20 GMT  
		Size: 8.3 KB (8324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598efee125341cd2a85d3613124625ecfb4d30f5c04825898faa678616c655f4`  
		Last Modified: Tue, 28 Sep 2021 11:58:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bd58bdf9a7a50e02d52f24a59ded137bf781c70175d3f72fa4b7a566e0934e`  
		Last Modified: Tue, 28 Sep 2021 11:58:20 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac726345f96ca8825fcf79b468e24f8cfa43e872b01ab5b6d38859e0b2abb72`  
		Last Modified: Tue, 28 Sep 2021 11:58:20 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; 386

```console
$ docker pull postgres@sha256:e4f0f65acba8d43fe0c9fd700c8905d011b75ec8477ff8c6c2cd93d0b409f0be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (109995932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56c19f118bb0a91de1a011a4925bba2d758a99e25c501a495b49f625f37924c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:46 GMT
ADD file:6c8a44184bf1d38b16f52d58ecb80d627ab86fce72a78b094170535fe1f76ad0 in / 
# Fri, 03 Sep 2021 00:42:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 16:04:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 16:04:13 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 03 Sep 2021 16:04:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 16:04:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 16:04:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 03 Sep 2021 16:04:50 GMT
ENV LANG=en_US.utf8
# Fri, 03 Sep 2021 16:04:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 16:05:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 16:05:08 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Fri, 03 Sep 2021 16:05:08 GMT
ENV PG_MAJOR=11
# Fri, 03 Sep 2021 16:05:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Fri, 03 Sep 2021 16:05:09 GMT
ENV PG_VERSION=11.13-1.pgdg90+1
# Fri, 03 Sep 2021 16:05:40 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 03 Sep 2021 16:05:41 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 03 Sep 2021 16:05:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 03 Sep 2021 16:05:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 03 Sep 2021 16:05:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 03 Sep 2021 16:05:44 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 03 Sep 2021 16:05:44 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 03 Sep 2021 16:05:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 16:05:44 GMT
STOPSIGNAL SIGINT
# Fri, 03 Sep 2021 16:05:45 GMT
EXPOSE 5432
# Fri, 03 Sep 2021 16:05:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0b43614231856f083f6dc06bd012a7ac7ff26410a945ea25d4c887e8218a878c`  
		Last Modified: Fri, 03 Sep 2021 00:53:23 GMT  
		Size: 23.2 MB (23156443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abea021c5bc89b9f765dd715203d1385b53a29ccfa57f89bcd984005cf69c726`  
		Last Modified: Fri, 03 Sep 2021 16:14:45 GMT  
		Size: 4.8 MB (4811150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a98f6a5975361064b7aeb87d1b9d605c8de7dbe54b5cd6fc8a79a05b3dfd0f8`  
		Last Modified: Fri, 03 Sep 2021 16:14:42 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838d0a09d7215471a71ef652e21e61fdb937b1ed8bec98d0ab985e8231bad43a`  
		Last Modified: Fri, 03 Sep 2021 16:14:43 GMT  
		Size: 1.4 MB (1382508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ee70d258a0c0b0a9b70578eea4506ef1e0d9c2957b6d53c71d3da95adfde2f`  
		Last Modified: Fri, 03 Sep 2021 16:14:43 GMT  
		Size: 6.2 MB (6185570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fd2706bb58d86695a5979067348a92b7efa5d06c3fa2d270f514e79881239d`  
		Last Modified: Fri, 03 Sep 2021 16:14:40 GMT  
		Size: 393.3 KB (393335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c646f28e6bd0662e1b06bbc1a601e2f95e19182e9645749540f1a8e7092a49`  
		Last Modified: Fri, 03 Sep 2021 16:14:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff53030bfd0020aeb52e4e9f505cb48941c20105c32895230eb4985ebb7c8e8`  
		Last Modified: Fri, 03 Sep 2021 16:14:39 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844583dd981846dc41012e3688268cc51b0c33ae96ca1e51ffd63374a76e8ed`  
		Last Modified: Fri, 03 Sep 2021 16:15:01 GMT  
		Size: 74.0 MB (74046578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926d9dfad832e60871e469409b735142a925b23a0352bea5570c0b33ba733b4c`  
		Last Modified: Fri, 03 Sep 2021 16:14:37 GMT  
		Size: 8.3 KB (8321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b100a60b183386c8bdad9ec3e5ddd5dafaf4d7c3bdd88d78582b1b4ee8ed4a`  
		Last Modified: Fri, 03 Sep 2021 16:14:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b575df192f638d19bf02e15f27779fb8cd16d366d3100f4bf4d6d52a1afbc3ea`  
		Last Modified: Fri, 03 Sep 2021 16:14:37 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7953550098837db92523cf2838e28592f082ba7e623fd3f57e540820572efd5`  
		Last Modified: Fri, 03 Sep 2021 16:14:37 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
