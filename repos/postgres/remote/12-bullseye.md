## `postgres:12-bullseye`

```console
$ docker pull postgres@sha256:d0724a3f2ad0ad477c0bac66dd47eed5d58cb2e0ba6811909eada59f8389d364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `postgres:12-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:d3ee6dedbe09fdf1febfb439fefe8016b012564727e017d47fefa3003a17cc8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c278af658a7eb90a63b684437c156c2656263e0d5693df92fafcb32b75c323b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:39:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 04:39:38 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 09 Feb 2023 04:39:38 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Feb 2023 04:39:47 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 09 Feb 2023 04:39:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 09 Feb 2023 04:39:54 GMT
ENV LANG=en_US.utf8
# Thu, 09 Feb 2023 04:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 04:39:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 09 Feb 2023 04:39:59 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 09 Feb 2023 04:41:33 GMT
ENV PG_MAJOR=12
# Thu, 09 Feb 2023 04:41:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 11 Feb 2023 05:11:58 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Sat, 11 Feb 2023 05:12:16 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 11 Feb 2023 05:12:18 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 11 Feb 2023 05:12:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 11 Feb 2023 05:12:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 11 Feb 2023 05:12:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 11 Feb 2023 05:12:19 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 11 Feb 2023 05:12:19 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:12:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:12:19 GMT
STOPSIGNAL SIGINT
# Sat, 11 Feb 2023 05:12:19 GMT
EXPOSE 5432
# Sat, 11 Feb 2023 05:12:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a54e59e691b29df361577e6c5b4d32fa6d2fa9039ad55f293d392f261afd68`  
		Last Modified: Thu, 09 Feb 2023 04:43:11 GMT  
		Size: 4.4 MB (4414957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce7f8df2b36f15fa7e09f22a197cb272923063dab7c0164c918505c22bfbfbb`  
		Last Modified: Thu, 09 Feb 2023 04:43:10 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30287ef02b9d1aa20483a1cb8af5136c17747081a4508cbbf9843dd960b7338`  
		Last Modified: Thu, 09 Feb 2023 04:43:10 GMT  
		Size: 1.5 MB (1471400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1f0e9024d8067e86a5c358052285b986b7d113e4ebe2bf5534188547ba0150`  
		Last Modified: Thu, 09 Feb 2023 04:43:09 GMT  
		Size: 8.0 MB (8045261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0a68628bceef9a8e7a7bad7a51a39ef4bea0e4d84449a54c8217486586591b`  
		Last Modified: Thu, 09 Feb 2023 04:43:08 GMT  
		Size: 1.3 MB (1261167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b11818cae32e3bc189ab44f009297a2545c3b3fac7eb95c9c15201fda30080`  
		Last Modified: Thu, 09 Feb 2023 04:43:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48111fe612c159d653ed7b96e5d6eb784f7b49fa920f66a17bbff924333b28c8`  
		Last Modified: Thu, 09 Feb 2023 04:43:08 GMT  
		Size: 3.2 KB (3199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80b16d65234095a42db12756bce3a2a10db28b124910800e45b9401207ea5d9`  
		Last Modified: Sat, 11 Feb 2023 05:21:52 GMT  
		Size: 89.7 MB (89652038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19fad3d1049c29365c44dd68c3ab70cf7888b7d22d63380ec3eaa3646883047`  
		Last Modified: Sat, 11 Feb 2023 05:21:40 GMT  
		Size: 9.0 KB (9022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf810218405286ed32f365a76aacaa2cc6deff3d9fdc25dd93d04c39641d940b`  
		Last Modified: Sat, 11 Feb 2023 05:21:39 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b314ffacaea5344c8c139ea11bfdb489037b093004c5243918ec008da9df6f`  
		Last Modified: Sat, 11 Feb 2023 05:21:40 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee35dbe1779365060689a5c87729c22658b1c1ec5ae141b33732e41a6956b88`  
		Last Modified: Sat, 11 Feb 2023 05:21:39 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:ed082ac5e35d04a60d84cce035ac91e0639d7bf890549aa88ceb1eaf82f6d641
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129535873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3f1620c47dae3a72e5c4e75619d81d8ace490c73fe228603f1bdda1d33c784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 05:31:24 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 01 Mar 2023 05:31:24 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 05:31:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 05:31:41 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 01 Mar 2023 05:31:41 GMT
ENV LANG=en_US.utf8
# Wed, 01 Mar 2023 05:31:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:31:48 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 05:31:49 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 06:13:15 GMT
ENV PG_MAJOR=12
# Wed, 01 Mar 2023 06:13:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Wed, 01 Mar 2023 06:13:15 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Wed, 01 Mar 2023 06:25:44 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 01 Mar 2023 06:25:46 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 01 Mar 2023 06:25:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 01 Mar 2023 06:25:47 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 01 Mar 2023 06:25:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 01 Mar 2023 06:25:48 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 01 Mar 2023 06:25:49 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Wed, 01 Mar 2023 06:25:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 06:25:49 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 06:25:50 GMT
EXPOSE 5432
# Wed, 01 Mar 2023 06:25:50 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a220700c1d34fe296a861acd3a7f7049210502075fb0aeae1b36dfba9da5a8e5`  
		Last Modified: Wed, 01 Mar 2023 06:39:13 GMT  
		Size: 4.1 MB (4096493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeefb5d270ed0e8861ce65e9d287a93263255ed286f949d821cdd4f5ff5abfc5`  
		Last Modified: Wed, 01 Mar 2023 06:39:12 GMT  
		Size: 1.8 KB (1793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad964d8ff65d411695ba5e33fbe39cdb03bcb59dc4e0c1e362ca2b3a49023455`  
		Last Modified: Wed, 01 Mar 2023 06:39:12 GMT  
		Size: 1.4 MB (1448661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6509bf5b97b335652c13742f70f6c488f0b8e5c6875311c5e65d38631511fdf`  
		Last Modified: Wed, 01 Mar 2023 06:39:12 GMT  
		Size: 8.0 MB (8045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7ee417e8f9ba665e97796719afee8c76a83fd14155df5e72b9684a8771a27`  
		Last Modified: Wed, 01 Mar 2023 06:39:10 GMT  
		Size: 1.3 MB (1257266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77fb29685e977ea2db144cf8bba9383b52519cc9348ee45f1d598335621f240a`  
		Last Modified: Wed, 01 Mar 2023 06:39:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cd6218816df1ea7717715f7c25168d977fa687f2e3f4d4ea2c9522fbf3f5ef`  
		Last Modified: Wed, 01 Mar 2023 06:39:09 GMT  
		Size: 3.2 KB (3193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11c404ec70d11b160ed5777cf6520154b0f862a0b54e4f6ced5a360c31c85bd`  
		Last Modified: Wed, 01 Mar 2023 06:41:06 GMT  
		Size: 85.8 MB (85753304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d8992c0a14038c8c2c3f34875ad1cfd93226da450c81f2334dcdcbf9b9ae48`  
		Last Modified: Wed, 01 Mar 2023 06:40:53 GMT  
		Size: 9.0 KB (9031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c711f86865b6057d32fa55451b8d97d45877aa505ea529d7192db4287a6ebc9a`  
		Last Modified: Wed, 01 Mar 2023 06:40:52 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e550ba123eccafd830c0e134582bd742b801ca6df968c6dd9ec42b2b1b2626cd`  
		Last Modified: Wed, 01 Mar 2023 06:40:53 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc5486701bd7b026b84cb7331212f25c9c3d2714f2f28548aeae13773ec7135`  
		Last Modified: Wed, 01 Mar 2023 06:40:52 GMT  
		Size: 4.8 KB (4780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:20201af16fe04ab42f84d72b17c51fe56ea99274b1207eeccec2e04f18aa8a7a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124294456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a26972e9ec85a3cd299293591be5e2b94422b109772a87b603a59746a97b2d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:14:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 13:14:57 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 09 Feb 2023 13:14:57 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Feb 2023 13:15:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 09 Feb 2023 13:15:13 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 09 Feb 2023 13:15:14 GMT
ENV LANG=en_US.utf8
# Thu, 09 Feb 2023 13:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:15:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 09 Feb 2023 13:15:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 09 Feb 2023 13:58:55 GMT
ENV PG_MAJOR=12
# Thu, 09 Feb 2023 13:58:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Fri, 10 Feb 2023 19:52:43 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Fri, 10 Feb 2023 20:05:38 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 10 Feb 2023 20:05:39 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 10 Feb 2023 20:05:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 10 Feb 2023 20:05:40 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 10 Feb 2023 20:05:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 10 Feb 2023 20:05:41 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 10 Feb 2023 20:05:41 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Fri, 10 Feb 2023 20:05:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 20:05:41 GMT
STOPSIGNAL SIGINT
# Fri, 10 Feb 2023 20:05:41 GMT
EXPOSE 5432
# Fri, 10 Feb 2023 20:05:41 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98d6d70c0121f76ebe7fd7f7c785dd228a22bef1146f8bdea856cbcf872e1a2`  
		Last Modified: Thu, 09 Feb 2023 14:27:14 GMT  
		Size: 3.7 MB (3717249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b956de2c93c5f193493bf6a7c556c28ab469d46e35659ea42179dd2465ace65c`  
		Last Modified: Thu, 09 Feb 2023 14:27:12 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87aa518ea997f79e26f1f6caeb8b6e8d8f0b85ff9bb8b415502ebd67907cb89c`  
		Last Modified: Thu, 09 Feb 2023 14:27:13 GMT  
		Size: 1.4 MB (1438720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c709a9d376db71baa9ac8e3fd7fa2ccad20e30ac3b44560243b82af26937812b`  
		Last Modified: Thu, 09 Feb 2023 14:27:12 GMT  
		Size: 8.0 MB (8045168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b617296d17a741940a578ef84c0ffcc83a8deab3b8e8987f1edb39ac395e7e86`  
		Last Modified: Thu, 09 Feb 2023 14:27:10 GMT  
		Size: 1.1 MB (1131218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff0c970066903b6248a85afad32a2f3573a1de80c5746975c05fefea46651c8`  
		Last Modified: Thu, 09 Feb 2023 14:27:10 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249d453676144db33f665ca9dddf80f22e9683914be7783aa3a045ab3c19d4b4`  
		Last Modified: Thu, 09 Feb 2023 14:27:10 GMT  
		Size: 3.2 KB (3168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859b392210412b309919d941327b165ed2561269caeace32f91f58104464c623`  
		Last Modified: Fri, 10 Feb 2023 20:29:45 GMT  
		Size: 83.4 MB (83365279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a69c706adc0ff8d465769c41915858acddd2c1e23f8e829e9c8730a272ce8d7`  
		Last Modified: Fri, 10 Feb 2023 20:29:31 GMT  
		Size: 9.0 KB (9027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c305fd61e42c8952f16fdb337eabac26abd45741e91d8e81307b5d1097336e9c`  
		Last Modified: Fri, 10 Feb 2023 20:29:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749751ee94456e8cff85e443fdb5ed2058ddf97ce1fa88a9f622bda1f721a526`  
		Last Modified: Fri, 10 Feb 2023 20:29:31 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fd7ea2c97d69aa2b4d922ab951387bf4fdca143e3cc31749f3a94cd5895c29`  
		Last Modified: Fri, 10 Feb 2023 20:29:31 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:766e4b5205b5653afe48c57b43f32600df86f2b87fd2a40c5b1a56c15d014683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131379813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4676034b854b8546d366750c9cd7fda0a522d8c2c40b95d262ec3eb8a7f7b948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 09:31:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 09:31:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 01 Mar 2023 09:31:34 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 09:31:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 09:31:48 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 01 Mar 2023 09:31:48 GMT
ENV LANG=en_US.utf8
# Wed, 01 Mar 2023 09:31:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 09:31:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 09:31:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 09:33:13 GMT
ENV PG_MAJOR=12
# Wed, 01 Mar 2023 09:33:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Wed, 01 Mar 2023 09:33:13 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Wed, 01 Mar 2023 09:33:28 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 01 Mar 2023 09:33:30 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 01 Mar 2023 09:33:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 01 Mar 2023 09:33:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 01 Mar 2023 09:33:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 01 Mar 2023 09:33:31 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 01 Mar 2023 09:33:31 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Wed, 01 Mar 2023 09:33:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 09:33:31 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 09:33:31 GMT
EXPOSE 5432
# Wed, 01 Mar 2023 09:33:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bda61a2fd3656f8cf71d54651a67afc51ea9013a12c2aed26f1e0dc2c4f11bf`  
		Last Modified: Wed, 01 Mar 2023 09:34:46 GMT  
		Size: 4.4 MB (4416224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71dece91b080cee3aadece35b6b2d5fb6a31a70d3886b0946b8032188b14cff`  
		Last Modified: Wed, 01 Mar 2023 09:34:44 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa8a57bd57fee24e35325424353b0eb14aeb85c56c9640d0b25a9f032630085`  
		Last Modified: Wed, 01 Mar 2023 09:34:44 GMT  
		Size: 1.4 MB (1403198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278e7f5a60e68f973de85538dfeb1394565ae4b0f1f573fcfc00984e1aa9dc9f`  
		Last Modified: Wed, 01 Mar 2023 09:34:44 GMT  
		Size: 8.0 MB (8045182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4e2b9db3494f040cd15b1293b90dec85976ebf3e5b3daf426c13bf1080c022`  
		Last Modified: Wed, 01 Mar 2023 09:34:43 GMT  
		Size: 1.2 MB (1249189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2dc87f9f55e131a9d2414f610ab3b56c97bbf91584a4c8955e08afc1a35844`  
		Last Modified: Wed, 01 Mar 2023 09:34:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cb5da6795676741ad765f56f16c68b0e08ce4541f0c1db545a36558e73f4f`  
		Last Modified: Wed, 01 Mar 2023 09:34:42 GMT  
		Size: 3.2 KB (3199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf40a6bb0a09674f50af48f7f95f27937477f6c3035377663ef5c365f3bb846c`  
		Last Modified: Wed, 01 Mar 2023 09:36:09 GMT  
		Size: 86.2 MB (86183926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bdb5d30ffa275e7dde1f8dcd77cb23ee4df68b2794bf642aa6c8ba2d5f1e01`  
		Last Modified: Wed, 01 Mar 2023 09:36:00 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210341a57b1c44cf1955e9b0090fa6733c69eb8e74b8d12efcdea6134e8285f0`  
		Last Modified: Wed, 01 Mar 2023 09:36:00 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ab37298fa2c53c153f19419a3dfb44b107f490be4e855f20a4874742f01255`  
		Last Modified: Wed, 01 Mar 2023 09:36:00 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8865c9d366655cc35a8be13298d8d0c7fe74a993b1c620bf6dd90e22b64312`  
		Last Modified: Wed, 01 Mar 2023 09:36:00 GMT  
		Size: 4.8 KB (4777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:3c86d6931d8bda39ea7e05d3d6398f6d20021e6ca2cc961bea674eca5995f78c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137853039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b011b792f88981ecd1f2d5ad881802d0cf59fe72f705e2eb6e6813525bc2ea5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:09:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 10:09:36 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 09 Feb 2023 10:09:37 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Feb 2023 10:09:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 09 Feb 2023 10:09:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 09 Feb 2023 10:09:53 GMT
ENV LANG=en_US.utf8
# Thu, 09 Feb 2023 10:09:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:09:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 09 Feb 2023 10:10:01 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 09 Feb 2023 10:50:44 GMT
ENV PG_MAJOR=12
# Thu, 09 Feb 2023 10:50:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Fri, 10 Feb 2023 20:30:27 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Fri, 10 Feb 2023 20:42:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 10 Feb 2023 20:42:40 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 10 Feb 2023 20:42:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 10 Feb 2023 20:42:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 10 Feb 2023 20:42:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 10 Feb 2023 20:42:43 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 10 Feb 2023 20:42:45 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Fri, 10 Feb 2023 20:42:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 20:42:46 GMT
STOPSIGNAL SIGINT
# Fri, 10 Feb 2023 20:42:47 GMT
EXPOSE 5432
# Fri, 10 Feb 2023 20:42:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee349b1f3becc7817bfd8d82a5f4aa49c315c613a2d2affe2ea2e23d51829dd`  
		Last Modified: Thu, 09 Feb 2023 11:16:47 GMT  
		Size: 4.6 MB (4607387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037b8b99e9fd1c5f2f3ad68b2030ded5b3b1748d70b95ff9b183a4178231e61a`  
		Last Modified: Thu, 09 Feb 2023 11:16:45 GMT  
		Size: 1.6 KB (1642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af44f2cdc39ec1f81a4dc0e81af5c3de507e8ba3e1db621502db354a52d07412`  
		Last Modified: Thu, 09 Feb 2023 11:16:46 GMT  
		Size: 1.4 MB (1446442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b036e9b531137a3b23f26a0e585a7ff468a83260c6645a3d22a471dab807e33d`  
		Last Modified: Thu, 09 Feb 2023 11:16:45 GMT  
		Size: 8.0 MB (8043353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6792e45a290bbc130214d22382683e1eb3b1d74459049eeccd87e604ded62dae`  
		Last Modified: Thu, 09 Feb 2023 11:16:44 GMT  
		Size: 1.0 MB (1027951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c248770b04df25042269961adb2876d17abfc2e64c308237dc3f177596eb23`  
		Last Modified: Thu, 09 Feb 2023 11:16:44 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6a493d5167e94180d21edb7ca42fa834925d4ec6896d6617844dfb270c3235`  
		Last Modified: Thu, 09 Feb 2023 11:16:44 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348dc4d86ea36acb12fc2708f8ac2b76abfa5f82fafdf7353669d68b1a9bc879`  
		Last Modified: Fri, 10 Feb 2023 21:05:46 GMT  
		Size: 90.3 MB (90312024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adb6bedd1555d2259eeef5e1087097319901db08546410f7b39b95f53234b51`  
		Last Modified: Fri, 10 Feb 2023 21:05:34 GMT  
		Size: 9.0 KB (9022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a74661c0508353c5ef9c6e0ee35c8e59f1e48370b0e501f9b619cee24da93a2`  
		Last Modified: Fri, 10 Feb 2023 21:05:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b855d87dd2e57c1b2171e221205cc6172676b685c422dd354fde297e003c02b2`  
		Last Modified: Fri, 10 Feb 2023 21:05:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a764e38ea4f2a46e90a9af8ee212c2cc3fa5711ee150093cb9f34f8af04c7d8e`  
		Last Modified: Fri, 10 Feb 2023 21:05:34 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:c32c372004f1a25cba009ef1e45a738b951f2d1ac9f908cc100a18bd5ae8a620
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130693986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9be41855e002e2eb2217691b0fcf3f9743f0da9ba4b5d71f2bafba4f2e8c8c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 09 Feb 2023 02:45:21 GMT
ADD file:68e11645a37c49c8f8f9d79ba579d0d192aaab78bb28059f07d69d56aa5ace71 in / 
# Thu, 09 Feb 2023 02:45:25 GMT
CMD ["bash"]
# Fri, 10 Feb 2023 20:31:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Feb 2023 20:31:25 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 10 Feb 2023 20:31:28 GMT
ENV GOSU_VERSION=1.16
# Fri, 10 Feb 2023 20:32:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 10 Feb 2023 20:32:31 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 10 Feb 2023 20:32:33 GMT
ENV LANG=en_US.utf8
# Fri, 10 Feb 2023 20:32:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 20:32:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 10 Feb 2023 20:33:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 10 Feb 2023 23:33:35 GMT
ENV PG_MAJOR=12
# Fri, 10 Feb 2023 23:33:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Fri, 10 Feb 2023 23:33:41 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Sat, 11 Feb 2023 00:28:33 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 11 Feb 2023 00:28:39 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 11 Feb 2023 00:28:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 11 Feb 2023 00:28:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 11 Feb 2023 00:28:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 11 Feb 2023 00:28:58 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 11 Feb 2023 00:29:01 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 11 Feb 2023 00:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 00:29:07 GMT
STOPSIGNAL SIGINT
# Sat, 11 Feb 2023 00:29:11 GMT
EXPOSE 5432
# Sat, 11 Feb 2023 00:29:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1b5516936229d6629ab88588210eb90edc2613c94e5952fd1caf9200284f298a`  
		Last Modified: Thu, 09 Feb 2023 02:53:48 GMT  
		Size: 29.6 MB (29634449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6db88899b0c8ecab88f3f98d7526ed3504ed47971b65b67c350fbdd8a911a7`  
		Last Modified: Sat, 11 Feb 2023 01:24:29 GMT  
		Size: 4.2 MB (4196331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e124a715415c19a5f741556cfe429385a9de9357e78228ece2b5d5b90b2a358`  
		Last Modified: Sat, 11 Feb 2023 01:24:24 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a232ed4e5dee4924f871059430611ff3f529eb174a51621e1c943fa6b18e76`  
		Last Modified: Sat, 11 Feb 2023 01:24:25 GMT  
		Size: 1.4 MB (1358240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c27cda5aba8f85b7ccc1df6646b14d68323acd4c5e0b885c2561853255c0379`  
		Last Modified: Sat, 11 Feb 2023 01:24:30 GMT  
		Size: 8.0 MB (8043767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9579e74a19019a8971d268f525a6d109a1286853ab84d5e89398f0e7cb62dc5`  
		Last Modified: Sat, 11 Feb 2023 01:24:22 GMT  
		Size: 1.1 MB (1089535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31055f1c9136f894be8c4123c243ddcda594c2648ba99cd3e447b7e16835045e`  
		Last Modified: Sat, 11 Feb 2023 01:24:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f660e2f28fb8b80f3a05aa065adb5b383d8cfbb5edb6f8d2f035e51770de410`  
		Last Modified: Sat, 11 Feb 2023 01:24:21 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c11c94ec53eb634de276fececbd1e720855fe72dc811e4d70ce8cc9cab1c176`  
		Last Modified: Sat, 11 Feb 2023 01:29:10 GMT  
		Size: 86.4 MB (86352653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09919bac79d4f772b34043fb5be03a8801493d680bfda4579b9378ea70bc3235`  
		Last Modified: Sat, 11 Feb 2023 01:28:14 GMT  
		Size: 9.0 KB (9024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7cecd279af0e89113a75971c8cdaa948e5e1766b87706ccdefe7b8ebf46d87`  
		Last Modified: Sat, 11 Feb 2023 01:28:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f88196097afaada1cc9bed97a1545ea015a7298a43365672c15d4114613d34`  
		Last Modified: Sat, 11 Feb 2023 01:28:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7e1ac5997742087360105ecd3e10639a69cf30f5cb95479405d1b7b2061aa0`  
		Last Modified: Sat, 11 Feb 2023 01:28:14 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:49e815d8b33f9b7e900d0a494bd66937a5fbd066470d0c9dd0d4697b9d031359
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145215984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dce7217909135c49ab602aa0e7d8971d067cd6b48174d8e0a931ca6fb14b4e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 10:41:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 10:41:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 01 Mar 2023 10:41:53 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 10:42:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 10:42:21 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 01 Mar 2023 10:42:22 GMT
ENV LANG=en_US.utf8
# Wed, 01 Mar 2023 10:42:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 10:42:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 10:42:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 10:46:00 GMT
ENV PG_MAJOR=12
# Wed, 01 Mar 2023 10:46:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Wed, 01 Mar 2023 10:46:01 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Wed, 01 Mar 2023 10:46:48 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 01 Mar 2023 10:46:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 01 Mar 2023 10:46:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 01 Mar 2023 10:46:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 01 Mar 2023 10:46:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 01 Mar 2023 10:46:59 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 01 Mar 2023 10:46:59 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Wed, 01 Mar 2023 10:46:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 10:47:00 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 10:47:00 GMT
EXPOSE 5432
# Wed, 01 Mar 2023 10:47:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d8462655b1129e0ea6f88db4bd45ca3b2b4c32259a0a437806e7044d00a4ca`  
		Last Modified: Wed, 01 Mar 2023 10:49:54 GMT  
		Size: 5.2 MB (5222848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4e78b9d3115474d435c9d141956ee21625865643385703b3b9cc12176d397d`  
		Last Modified: Wed, 01 Mar 2023 10:49:52 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0191a0363b8d6ebf45831b1acadce33b05a0816ecbc9fa65e5126d2f2a2333cc`  
		Last Modified: Wed, 01 Mar 2023 10:49:53 GMT  
		Size: 1.4 MB (1393213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d73b5f41cef667f267cf9f2d827cbb481a2fd2bf0ac5673474ba2d09d13c65`  
		Last Modified: Wed, 01 Mar 2023 10:49:53 GMT  
		Size: 8.0 MB (8045159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a8a36b8c92b4db1fa09d3a9ecc9365feffcf9ab3f1d31cd615ea82c3c67a14`  
		Last Modified: Wed, 01 Mar 2023 10:49:51 GMT  
		Size: 1.4 MB (1420143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c46c47a1d1815cb5b4098277fd08fae210d669a0b9f0a962aa32fd6dda4df0`  
		Last Modified: Wed, 01 Mar 2023 10:49:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bba8fb4d18d6b0799212a5fcc8d27f0fba45c8ccbb8fe1ee8c362fcd5486a7`  
		Last Modified: Wed, 01 Mar 2023 10:49:50 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4a87b425293c2e758f408e6e18b0abc0a65ad1746b0c19c3dce70342165bac`  
		Last Modified: Wed, 01 Mar 2023 10:52:27 GMT  
		Size: 93.8 MB (93827229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a301331b71dc09760204576397fb590499d020b642991a875254f3df38e4c4fe`  
		Last Modified: Wed, 01 Mar 2023 10:52:04 GMT  
		Size: 9.0 KB (9022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5b12dd37f6d94b0db47decdd857e0bd8e09d0db09b9b633b690e15b614056a`  
		Last Modified: Wed, 01 Mar 2023 10:52:04 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affcce1cb1bd202f22c4215e4cccc2f57323c2deb954fad4c08fb79d0d2362b8`  
		Last Modified: Wed, 01 Mar 2023 10:52:04 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe52493dc5940eba9b6a0d5153a13c6bf34332e2a0743662f864572fd8f16223`  
		Last Modified: Wed, 01 Mar 2023 10:52:04 GMT  
		Size: 4.8 KB (4781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:8a34e31e91e28f68499932db6f92f13d75e0153927d89fe2dbd3f99091ceb73f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140030748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd378271ac5cce7a982630df7bddb533d93d5634d0e64ac79f1dc9f9be31e2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:30 GMT
ADD file:01aa3de7444f0716938e0d85522be065193be4ffb6788b3190a0f4fefdbb8d65 in / 
# Wed, 01 Mar 2023 02:50:31 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 09:05:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 09:05:42 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 01 Mar 2023 09:05:43 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 09:05:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 09:05:56 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 01 Mar 2023 09:05:57 GMT
ENV LANG=en_US.utf8
# Wed, 01 Mar 2023 09:06:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 09:06:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 09:06:03 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 09:31:43 GMT
ENV PG_MAJOR=12
# Wed, 01 Mar 2023 09:31:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Wed, 01 Mar 2023 09:31:43 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Wed, 01 Mar 2023 09:41:06 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 01 Mar 2023 09:41:11 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 01 Mar 2023 09:41:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 01 Mar 2023 09:41:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 01 Mar 2023 09:41:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 01 Mar 2023 09:41:12 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 01 Mar 2023 09:41:12 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Wed, 01 Mar 2023 09:41:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 09:41:13 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 09:41:13 GMT
EXPOSE 5432
# Wed, 01 Mar 2023 09:41:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1118ca97a87fe3bd04ae9263ec7a9ad75bb035d9a7e6e8df8ff9d24049a1737a`  
		Last Modified: Wed, 01 Mar 2023 09:51:34 GMT  
		Size: 4.3 MB (4302229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7da5301ce65906246fa21b49664df805eb612b8b037b8249d89ae6d8f182b5`  
		Last Modified: Wed, 01 Mar 2023 09:51:33 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e542f06a58c7b141cc8ea937c17e8e7dd87c4990f75ea383e7ecc3e0065a9116`  
		Last Modified: Wed, 01 Mar 2023 09:51:33 GMT  
		Size: 1.4 MB (1436959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d99ca10d4e04d0a4cf224a607572991157223a4f8f0291e486e7a73389fc98`  
		Last Modified: Wed, 01 Mar 2023 09:51:33 GMT  
		Size: 8.1 MB (8099239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff77ec748068d08c205ddcbef7bb446f78a0510f9ac33329e559087c15a8132`  
		Last Modified: Wed, 01 Mar 2023 09:51:32 GMT  
		Size: 1.2 MB (1237940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b3897fb4871ab8c2e0d66e5b2ec7b6117def2c6f9d271b0109645e5b17e45b`  
		Last Modified: Wed, 01 Mar 2023 09:51:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b42c547d17d6316259b87aed8c757aafc94b78ff969a0cd95846018560746a`  
		Last Modified: Wed, 01 Mar 2023 09:51:32 GMT  
		Size: 3.2 KB (3196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883749dfbf0ce2d5d8a2c6bc4b58f8caee43378563f18f7169f87fc06b229702`  
		Last Modified: Wed, 01 Mar 2023 09:52:58 GMT  
		Size: 95.3 MB (95288235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fce2c6093323ae9649c970edc452c8ab96499ea62825572f222767ddeffb2b`  
		Last Modified: Wed, 01 Mar 2023 09:52:46 GMT  
		Size: 9.0 KB (9033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38577c9c4673f26c55b0008e418c848af49b6cb0cd51914ad9847515bf558d3c`  
		Last Modified: Wed, 01 Mar 2023 09:52:46 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79557d8f1647a99de744f90dbe751a32338654f6defc1347faffc8fb211f596d`  
		Last Modified: Wed, 01 Mar 2023 09:52:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9324dd76ce71b7c4b19a0751f1e43a60015b42693cedb749703e77b040970d`  
		Last Modified: Wed, 01 Mar 2023 09:52:46 GMT  
		Size: 4.8 KB (4779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
