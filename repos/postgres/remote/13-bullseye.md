## `postgres:13-bullseye`

```console
$ docker pull postgres@sha256:019c5e1e0a7fcb7b5032abcc1b5bfbdd4045a55eef00d33b762c9f7bd95fedd3
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

### `postgres:13-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:2d0e2546ee1d25b9db553e59a3ea4930e523e05df27d642add13624904eb5919
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136757296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3d8bd95dcae168fd82c147748b85cedf066e9f821189884fd0d594f8757da6`
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
# Thu, 09 Feb 2023 04:41:02 GMT
ENV PG_MAJOR=13
# Thu, 09 Feb 2023 04:41:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Sat, 11 Feb 2023 05:08:56 GMT
ENV PG_VERSION=13.10-1.pgdg110+1
# Sat, 11 Feb 2023 05:09:12 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 11 Feb 2023 05:09:13 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 11 Feb 2023 05:09:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 11 Feb 2023 05:09:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 11 Feb 2023 05:09:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 11 Feb 2023 05:09:15 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 11 Feb 2023 05:09:15 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:09:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:09:15 GMT
STOPSIGNAL SIGINT
# Sat, 11 Feb 2023 05:09:15 GMT
EXPOSE 5432
# Sat, 11 Feb 2023 05:09:15 GMT
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
	-	`sha256:53d17e3561d4d9a5857a5765884de3dbd619aa1692f4097a7a78f255a464213a`  
		Last Modified: Sat, 11 Feb 2023 05:21:00 GMT  
		Size: 90.1 MB (90133083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4574cb861f6aee05a0f2b5172df58cab7c548c784783201386d18140c00c4e35`  
		Last Modified: Sat, 11 Feb 2023 05:20:47 GMT  
		Size: 9.4 KB (9356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f24d68ef30dc12a7f04963fc2fa8cba81db6c9b738d7a1a6d78b6c5f8341e7a`  
		Last Modified: Sat, 11 Feb 2023 05:20:47 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bf55f1b69485da95d1c8ac2db21f740dbd9004af12a3df97bb44b90a48b0a1`  
		Last Modified: Sat, 11 Feb 2023 05:20:47 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4b4d1b8ce2f9588aaf1bf93e6f9505b9074f3c441227a21a3acdcf044cf95e`  
		Last Modified: Sat, 11 Feb 2023 05:20:47 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:7abae4b6a64cc7878b50b15f77ccdfbd2fe60e2dcdea5dd863fdf90bd9359b01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129979468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f67bb6b8b905d465e1dee38720889e55ef542dbfdab34f33d04d0170f5767c9e`
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
# Wed, 01 Mar 2023 06:00:05 GMT
ENV PG_MAJOR=13
# Wed, 01 Mar 2023 06:00:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 01 Mar 2023 06:00:06 GMT
ENV PG_VERSION=13.10-1.pgdg110+1
# Wed, 01 Mar 2023 06:13:04 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 01 Mar 2023 06:13:05 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 01 Mar 2023 06:13:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 01 Mar 2023 06:13:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 01 Mar 2023 06:13:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 01 Mar 2023 06:13:07 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 01 Mar 2023 06:13:07 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Wed, 01 Mar 2023 06:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 06:13:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 06:13:07 GMT
EXPOSE 5432
# Wed, 01 Mar 2023 06:13:07 GMT
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
	-	`sha256:b303d50d21981cd17d1efcf46b3bf2d256b66734fc953f980c54b0c118cc0d75`  
		Last Modified: Wed, 01 Mar 2023 06:40:35 GMT  
		Size: 86.2 MB (86196564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6564d643deed2b72579938eb24d49a97291ff5b75e578169abaf8df96b736c`  
		Last Modified: Wed, 01 Mar 2023 06:40:21 GMT  
		Size: 9.4 KB (9363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b60c1a9b135421d1f894c26c5942809a796879507f873e431825bd1f39cccf0`  
		Last Modified: Wed, 01 Mar 2023 06:40:21 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e90110ff42638c4ed30760fc88ddd69ee360111fb636fe77a8f48aa893116e7`  
		Last Modified: Wed, 01 Mar 2023 06:40:21 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f59e9bb071dcc89bce9481f883edf4d19c2dd3d4f53f5fffbcd2c41ec5fa44`  
		Last Modified: Wed, 01 Mar 2023 06:40:21 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:938701be939d6c7f649bc6e903e996aec0213dfe0d68d21fa314d18938ba977f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124710885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a5ae88ae933b5f708058febaf6a8ac5af747d428099df072dd2aa724f4e8e5e`
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
# Thu, 09 Feb 2023 13:44:49 GMT
ENV PG_MAJOR=13
# Thu, 09 Feb 2023 13:44:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 10 Feb 2023 19:36:13 GMT
ENV PG_VERSION=13.10-1.pgdg110+1
# Fri, 10 Feb 2023 19:49:35 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 10 Feb 2023 19:49:37 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 10 Feb 2023 19:49:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 10 Feb 2023 19:49:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 10 Feb 2023 19:49:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 10 Feb 2023 19:49:39 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 10 Feb 2023 19:49:39 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Fri, 10 Feb 2023 19:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 19:49:39 GMT
STOPSIGNAL SIGINT
# Fri, 10 Feb 2023 19:49:39 GMT
EXPOSE 5432
# Fri, 10 Feb 2023 19:49:39 GMT
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
	-	`sha256:1a9918a92d2e8aaacef49c5d142d9e22c7144681ed11923415a1755f42474b46`  
		Last Modified: Fri, 10 Feb 2023 20:28:40 GMT  
		Size: 83.8 MB (83781379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98aed3e5f0864a88ad04a2292e08a3d5bf81e984b7500e8a47b2c53112543be`  
		Last Modified: Fri, 10 Feb 2023 20:28:26 GMT  
		Size: 9.4 KB (9358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28191fb80f1e4e435e44fdc345193ea851ba831358a96c852c29ee5475d0701`  
		Last Modified: Fri, 10 Feb 2023 20:28:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e53bc80d4c363e7c6630188b2b953b759e4e11a5209f39e204b9921bb9db87`  
		Last Modified: Fri, 10 Feb 2023 20:28:26 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4bffcb2cb975012c134d01b73b87e6114581f84a0ee7f35df5be40075ba75b`  
		Last Modified: Fri, 10 Feb 2023 20:28:26 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:ffc3fcedf4d396efb12d782eeb52305e80bd52c9889942b4ae0d59e3b1d3ffbd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131837639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:465529af49f420c87a84bea43233419bb0bed8f8e17d3f56b3fa6a84eea831ec`
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
# Wed, 01 Mar 2023 09:32:48 GMT
ENV PG_MAJOR=13
# Wed, 01 Mar 2023 09:32:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 01 Mar 2023 09:32:48 GMT
ENV PG_VERSION=13.10-1.pgdg110+1
# Wed, 01 Mar 2023 09:33:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 01 Mar 2023 09:33:04 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 01 Mar 2023 09:33:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 01 Mar 2023 09:33:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 01 Mar 2023 09:33:05 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 01 Mar 2023 09:33:06 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 01 Mar 2023 09:33:06 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Wed, 01 Mar 2023 09:33:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 09:33:06 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 09:33:06 GMT
EXPOSE 5432
# Wed, 01 Mar 2023 09:33:06 GMT
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
	-	`sha256:45680b708b7963dc80e10e211ab2d7adf0079ed156ad490cd383a8b32313373a`  
		Last Modified: Wed, 01 Mar 2023 09:35:45 GMT  
		Size: 86.6 MB (86641427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2cc6e043a5a229fc9d5ddc7f51c269d660398931a6264097ff2f8c208521cb`  
		Last Modified: Wed, 01 Mar 2023 09:35:36 GMT  
		Size: 9.4 KB (9352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7feff50f7f9481170d8d9701a5fd9aee246395dcd046a97d712b3a5f84e5b`  
		Last Modified: Wed, 01 Mar 2023 09:35:36 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9744b3d4e4febb64ad058fe31f63eff9851c5ed8b7abd28f77155b41e7fe0fe0`  
		Last Modified: Wed, 01 Mar 2023 09:35:36 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaff125fb68f5115da103906eeff0dd7fcacde0a5951d3d15391bab6c10f6199`  
		Last Modified: Wed, 01 Mar 2023 09:35:36 GMT  
		Size: 4.8 KB (4776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:113906e5d916d1534ae0b360bd6c14aef3adc58e2295050bdaa5831e34ff05aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138361633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e915fb19a6e00e63b4f5c8b557090caa58cdbf554ef43e462f9578bbfc7f56`
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
# Thu, 09 Feb 2023 10:37:40 GMT
ENV PG_MAJOR=13
# Thu, 09 Feb 2023 10:37:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 10 Feb 2023 20:14:29 GMT
ENV PG_VERSION=13.10-1.pgdg110+1
# Fri, 10 Feb 2023 20:27:06 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 10 Feb 2023 20:27:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 10 Feb 2023 20:27:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 10 Feb 2023 20:27:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 10 Feb 2023 20:27:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 10 Feb 2023 20:27:10 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 10 Feb 2023 20:27:12 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Fri, 10 Feb 2023 20:27:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 20:27:13 GMT
STOPSIGNAL SIGINT
# Fri, 10 Feb 2023 20:27:14 GMT
EXPOSE 5432
# Fri, 10 Feb 2023 20:27:15 GMT
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
	-	`sha256:ddf22f15c14c9625f3c3975791b38b9ee0fd21a0ccee7abdb1ab9623486db2f1`  
		Last Modified: Fri, 10 Feb 2023 21:04:46 GMT  
		Size: 90.8 MB (90820277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c60822b2dd11378314a9f50200219116befcaf87715af7cb639f181459943c`  
		Last Modified: Fri, 10 Feb 2023 21:04:34 GMT  
		Size: 9.4 KB (9359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb969651860bd593f925954675bb1fbeb240b933cdd7bd9eef1fe734d9e5ad44`  
		Last Modified: Fri, 10 Feb 2023 21:04:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e525a15ef9439f5e03e6c8e981bb4e34beb277def4033c3de6fdfde5e81ccb13`  
		Last Modified: Fri, 10 Feb 2023 21:04:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58505181194d1850552e356afa6f2e37069c85ddca684e0709438e565e0043d`  
		Last Modified: Fri, 10 Feb 2023 21:04:34 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:c8f892d380ca078754c7d648c50a84ce435a27448c8302c60b7bf639ed5b18ab
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131138486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8f95147667ad6e1d4db4edca6873474593f316b9aa6b1e6c60b17434ebffc49`
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
# Fri, 10 Feb 2023 22:35:20 GMT
ENV PG_MAJOR=13
# Fri, 10 Feb 2023 22:35:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 10 Feb 2023 22:35:25 GMT
ENV PG_VERSION=13.10-1.pgdg110+1
# Fri, 10 Feb 2023 23:32:46 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 10 Feb 2023 23:32:52 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 10 Feb 2023 23:32:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 10 Feb 2023 23:33:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 10 Feb 2023 23:33:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 10 Feb 2023 23:33:10 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 10 Feb 2023 23:33:13 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Fri, 10 Feb 2023 23:33:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 23:33:20 GMT
STOPSIGNAL SIGINT
# Fri, 10 Feb 2023 23:33:24 GMT
EXPOSE 5432
# Fri, 10 Feb 2023 23:33:27 GMT
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
	-	`sha256:b95bcc4bf4a856f8db00b3b9437febad0daf3b7ca25b0e2820d822370293fd4f`  
		Last Modified: Sat, 11 Feb 2023 01:27:57 GMT  
		Size: 86.8 MB (86796814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290c9e7e6ca1dba8783279a7429964403b04acb9fbf35dcff74b728ffc27de1a`  
		Last Modified: Sat, 11 Feb 2023 01:27:00 GMT  
		Size: 9.4 KB (9362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037c73a53afb239d2123eab5c62600d6cefc81f965904ac91ce396cc9df0cb2c`  
		Last Modified: Sat, 11 Feb 2023 01:27:00 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86b9783282f28eb6531f067c715e682e502498fd748ee50016fdc4b192d8145`  
		Last Modified: Sat, 11 Feb 2023 01:27:00 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076bde2504bd72d1ae769910da9f18133b8964629d181264edbcb55403fb7709`  
		Last Modified: Sat, 11 Feb 2023 01:27:00 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:9071740d40febac691482b388df4045a19322693af81108c498b902a8bc22f0e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.7 MB (145707104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce87c9515e8d55dc38fba70f6cef00bbf995eded9104b412082c93f426b0a063`
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
# Wed, 01 Mar 2023 10:45:06 GMT
ENV PG_MAJOR=13
# Wed, 01 Mar 2023 10:45:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 01 Mar 2023 10:45:07 GMT
ENV PG_VERSION=13.10-1.pgdg110+1
# Wed, 01 Mar 2023 10:45:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 01 Mar 2023 10:45:45 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 01 Mar 2023 10:45:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 01 Mar 2023 10:45:47 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 01 Mar 2023 10:45:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 01 Mar 2023 10:45:48 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 01 Mar 2023 10:45:49 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Wed, 01 Mar 2023 10:45:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 10:45:49 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 10:45:50 GMT
EXPOSE 5432
# Wed, 01 Mar 2023 10:45:50 GMT
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
	-	`sha256:5e08e4251eb2e65022d390191e0a7f16f6cfca9690d6d0e4a755503ba6bfc2ae`  
		Last Modified: Wed, 01 Mar 2023 10:51:44 GMT  
		Size: 94.3 MB (94318012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542142125a5d9458a16ca74bf6bc4a871438f58d4e523f218aab38b6352a6cee`  
		Last Modified: Wed, 01 Mar 2023 10:51:22 GMT  
		Size: 9.4 KB (9361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a199502a832abc60a03e199fb930461f833bc23aea6403e70ba54b0fd1b5b3`  
		Last Modified: Wed, 01 Mar 2023 10:51:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d86703daad527ca520ca18bf1e62e038da6d30d005f6317c86fc580493def32`  
		Last Modified: Wed, 01 Mar 2023 10:51:22 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbb113ebe4da78ae49b09f389d6435032aab24d88ec6312fe5c7a30832dfa45`  
		Last Modified: Wed, 01 Mar 2023 10:51:22 GMT  
		Size: 4.8 KB (4780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:48f8277c7b876cf62cf1a218604a9cb90ffc2f4af7899dcc6c853632f3ff24b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140387149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223dcdbf8246c0aa333de00332fbd20ae50055dcb432c42de9beffa36ef390ff`
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
# Wed, 01 Mar 2023 09:21:54 GMT
ENV PG_MAJOR=13
# Wed, 01 Mar 2023 09:21:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 01 Mar 2023 09:21:54 GMT
ENV PG_VERSION=13.10-1.pgdg110+1
# Wed, 01 Mar 2023 09:31:23 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 01 Mar 2023 09:31:28 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 01 Mar 2023 09:31:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 01 Mar 2023 09:31:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 01 Mar 2023 09:31:29 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 01 Mar 2023 09:31:29 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 01 Mar 2023 09:31:30 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Wed, 01 Mar 2023 09:31:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 09:31:30 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 09:31:30 GMT
EXPOSE 5432
# Wed, 01 Mar 2023 09:31:30 GMT
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
	-	`sha256:2256151931666ab048251759d2b85cfb2750a8c16fd104dba51c35138cc432d3`  
		Last Modified: Wed, 01 Mar 2023 09:52:31 GMT  
		Size: 95.6 MB (95644309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a3c654d197e227bb1d46133af22f1f57569aeeccd42627449dc0b6488f01a5`  
		Last Modified: Wed, 01 Mar 2023 09:52:18 GMT  
		Size: 9.4 KB (9362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b6a314c3957129200107e6859926b3fc53ce2b72b6ad9bd96885ab788118c0`  
		Last Modified: Wed, 01 Mar 2023 09:52:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ef4935daa8e32b55f92ccc4a5f7b4d6670434d7627b36b06b185f6961ce8a0`  
		Last Modified: Wed, 01 Mar 2023 09:52:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e290b1bcb9f84b4473c2baebf4ec4d39fcff60fdc9a0596896597dac252c1962`  
		Last Modified: Wed, 01 Mar 2023 09:52:18 GMT  
		Size: 4.8 KB (4778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
