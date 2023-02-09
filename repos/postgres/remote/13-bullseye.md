## `postgres:13-bullseye`

```console
$ docker pull postgres@sha256:e217df70d73f2d5fbe9f8dc56ab7ae4c364cfdafcf5c8170dfdb864d35fd1b7a
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
$ docker pull postgres@sha256:f5911875bf2d18c585a5f245f6596d946d28eabddeffd809ac52ca5720c7c5b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136724338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7424fa040a0f563c856c523e05d504c7b15c8908b36a3e2fa989e07c61ea552`
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
# Thu, 09 Feb 2023 04:41:02 GMT
ENV PG_VERSION=13.9-1.pgdg110+1
# Thu, 09 Feb 2023 04:41:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 09 Feb 2023 04:41:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 09 Feb 2023 04:41:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 09 Feb 2023 04:41:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Feb 2023 04:41:23 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 09 Feb 2023 04:41:23 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Feb 2023 04:41:23 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:41:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 04:41:24 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 04:41:24 GMT
EXPOSE 5432
# Thu, 09 Feb 2023 04:41:24 GMT
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
	-	`sha256:20a002889a9a7719dad49a1e6fc18a9a42e3e5e2af49a055bbf00789aad8aefc`  
		Last Modified: Thu, 09 Feb 2023 04:44:21 GMT  
		Size: 90.1 MB (90100125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad2b1f0e9bde5bea69b456b7d43f559a2e53653990a412891350da6924c3f3c`  
		Last Modified: Thu, 09 Feb 2023 04:44:09 GMT  
		Size: 9.4 KB (9360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b37effddbb9c75d070b31b3bd435bd448ce5eb386b324fac93e0c2da146018ef`  
		Last Modified: Thu, 09 Feb 2023 04:44:09 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e051487b101de9ba8cab9523a6814c0a0f0f96d580d142ce57d2078d13a8c2bb`  
		Last Modified: Thu, 09 Feb 2023 04:44:09 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0448fbfd5a3edd01d26700a921e9f1cff7e2cb7dc523138d957baa31aff7caf`  
		Last Modified: Thu, 09 Feb 2023 04:44:09 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:5b1c1750a0a28ed447950d36ea412f2e61ca174a4345bb21315c8b8d31918446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129951329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5840f3d44df096e1a7320749bf1c456e83625857090d8c16bb98e8b8a3bc4f32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:32 GMT
ADD file:fcf4deede0eb98d96d8657dfb1b0918a2c3d35f16d4858dd9e75c843edeff166 in / 
# Thu, 09 Feb 2023 02:00:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:41:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 03:41:55 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 09 Feb 2023 03:41:55 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Feb 2023 03:42:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 09 Feb 2023 03:42:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 09 Feb 2023 03:42:15 GMT
ENV LANG=en_US.utf8
# Thu, 09 Feb 2023 03:42:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 03:42:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 09 Feb 2023 03:42:23 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 09 Feb 2023 04:14:52 GMT
ENV PG_MAJOR=13
# Thu, 09 Feb 2023 04:14:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Thu, 09 Feb 2023 04:14:52 GMT
ENV PG_VERSION=13.9-1.pgdg110+1
# Thu, 09 Feb 2023 04:30:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 09 Feb 2023 04:30:05 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 09 Feb 2023 04:30:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 09 Feb 2023 04:30:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Feb 2023 04:30:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 09 Feb 2023 04:30:08 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Feb 2023 04:30:08 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:30:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 04:30:09 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 04:30:09 GMT
EXPOSE 5432
# Thu, 09 Feb 2023 04:30:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:886a7482403a267f98b84e4a9f9ede516bac1fe7eb82ff570dabbb0b297d5b53`  
		Last Modified: Thu, 09 Feb 2023 02:05:42 GMT  
		Size: 28.9 MB (28916292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b087795072fade3977475f93987d623d65d8219ce281d906ec76e8371afc3c5f`  
		Last Modified: Thu, 09 Feb 2023 05:00:56 GMT  
		Size: 4.1 MB (4096465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcf43b2a93980ee76d576de9165eec379df5caa41f751851c7d5a9c279c729a`  
		Last Modified: Thu, 09 Feb 2023 05:00:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f948fea09a0223880c5d16dfd84def27a5d3b7b59d8152789ee7e2e24d25fd1`  
		Last Modified: Thu, 09 Feb 2023 05:00:55 GMT  
		Size: 1.4 MB (1448634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6452f5b7fe1ac9c11e02234fd0f5bbb708ae446a6aa45f629ad8b8951dd135aa`  
		Last Modified: Thu, 09 Feb 2023 05:00:55 GMT  
		Size: 8.0 MB (8045126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ba4d457d028c0fcea811f9591e006755934776d10457db00394c3fe0d0b44b`  
		Last Modified: Thu, 09 Feb 2023 05:00:53 GMT  
		Size: 1.3 MB (1257257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1a93f3e6f2f07652410f224efe3d80352f7355079c1322cb14aa8c8e3f394b`  
		Last Modified: Thu, 09 Feb 2023 05:00:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0cbfff446dd8db9f240a63bd0ce4a5b48e009797ab9ce5055abf948fbff2a6`  
		Last Modified: Thu, 09 Feb 2023 05:00:52 GMT  
		Size: 3.2 KB (3169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03732f429190420552687258ae421b0099fc4563a4973201568f1452ad2ca6f1`  
		Last Modified: Thu, 09 Feb 2023 05:02:28 GMT  
		Size: 86.2 MB (86168068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d60477b47b5f413ab2ee7c69dd53e514529867f62849966dedf21ac4665fba`  
		Last Modified: Thu, 09 Feb 2023 05:02:11 GMT  
		Size: 9.4 KB (9365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d458f52552fb6f77e07cd8bde5bcbbd90de2b4db72ed46f3117dfb1e7670318a`  
		Last Modified: Thu, 09 Feb 2023 05:02:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e319cd6d1b426e1dcf082e1a466e1765886b2308bfab9e7cbe6133b639f43db`  
		Last Modified: Thu, 09 Feb 2023 05:02:11 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49522ef4ffc9a38fa00c7274bb7d35941802988774d84c7684d539b3a051e07`  
		Last Modified: Thu, 09 Feb 2023 05:02:11 GMT  
		Size: 4.8 KB (4781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:3eb3abff3225316751f3edb76894fa1972b045d9b21d55edb456b6001cb0cad6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124654285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15a22163d6c1f84b58b709c894c44989f27655ea1c369f1891184cdda450b87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 19:01:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 19:01:10 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 04 Feb 2023 19:01:10 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Feb 2023 19:01:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 04 Feb 2023 19:01:26 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 04 Feb 2023 19:01:27 GMT
ENV LANG=en_US.utf8
# Sat, 04 Feb 2023 19:01:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 19:01:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 04 Feb 2023 19:01:33 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 04 Feb 2023 19:30:01 GMT
ENV PG_MAJOR=13
# Sat, 04 Feb 2023 19:30:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Sat, 04 Feb 2023 19:30:01 GMT
ENV PG_VERSION=13.9-1.pgdg110+1
# Sat, 04 Feb 2023 19:43:15 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 19:43:17 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 19:43:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 19:43:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 19:43:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 19:43:18 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 19:43:18 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 19:43:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 19:43:18 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 19:43:18 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 19:43:18 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797ef53469c4f829c65985e5a2569db1d06d046c6e68562794471c2c379b9fa0`  
		Last Modified: Sat, 04 Feb 2023 20:11:25 GMT  
		Size: 3.7 MB (3717197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a788fed3d123c8190d82d0a27474fd1813f46e9a31eeb045e9782dd10f7b19e6`  
		Last Modified: Sat, 04 Feb 2023 20:11:24 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7981b6f30e3f7d86a2392a60b4626c778c0d929132497fb339e49abca4e076`  
		Last Modified: Sat, 04 Feb 2023 20:11:25 GMT  
		Size: 1.4 MB (1438705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97379137d6cd069eaa9bbb5d8ae204d7ea6ec6511a89dd52eff886b0a7878c84`  
		Last Modified: Sat, 04 Feb 2023 20:11:24 GMT  
		Size: 8.0 MB (8045148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cf7dd8a24d0238a035d6244e4b8345e20de750b1b546e94af34b10add1beeb`  
		Last Modified: Sat, 04 Feb 2023 20:11:23 GMT  
		Size: 1.1 MB (1131182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75c2901532f515a2d31eb3d8b637b7470ed65bd323463f816595c7e1b8f22b7`  
		Last Modified: Sat, 04 Feb 2023 20:11:22 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e43256e02278734e882e2dea8d7b487a25823ad2e4591aa8a66449ff812319`  
		Last Modified: Sat, 04 Feb 2023 20:11:22 GMT  
		Size: 3.2 KB (3169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17c4f4fa49f045935420e583658eba2d33d1f17e6ca1c0f54cfd49e73f65684`  
		Last Modified: Sat, 04 Feb 2023 20:13:00 GMT  
		Size: 83.7 MB (83743085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9466c41d2ae6ccc8143e3f7923fd54a2173875c242cca42dd8f1b9db7ed984`  
		Last Modified: Sat, 04 Feb 2023 20:12:45 GMT  
		Size: 9.4 KB (9369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967ca6aa068c11da56925ceaf98a3d37fb376fc52fe57ae914d3f1fa9e565d22`  
		Last Modified: Sat, 04 Feb 2023 20:12:45 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d191bafc4c68d5edc7c7ea16d44389666035356f15426f7f0006d27cc3d489a`  
		Last Modified: Sat, 04 Feb 2023 20:12:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e91364979ef0ed64a975f2c99499eb953428e75c8bb05f31fb79b1f9036b5f6`  
		Last Modified: Sat, 04 Feb 2023 20:12:45 GMT  
		Size: 4.8 KB (4780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:c92dbc33e6af324bd460e17451e79327c07cd432231beb9ec4cabf278d689b03
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131785289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03eba566795496230325aa95321cd24b8a850cbdaeac14b88a3721f115df5e0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 13:25:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 13:25:17 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 04 Feb 2023 13:25:17 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Feb 2023 13:25:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 04 Feb 2023 13:25:32 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 04 Feb 2023 13:25:32 GMT
ENV LANG=en_US.utf8
# Sat, 04 Feb 2023 13:25:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 13:25:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 04 Feb 2023 13:25:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 04 Feb 2023 13:26:26 GMT
ENV PG_MAJOR=13
# Sat, 04 Feb 2023 13:26:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Sat, 04 Feb 2023 13:26:26 GMT
ENV PG_VERSION=13.9-1.pgdg110+1
# Sat, 04 Feb 2023 13:26:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 13:26:42 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 13:26:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 13:26:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 13:26:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 13:26:44 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 13:26:44 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 13:26:44 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 13:26:44 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 13:26:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738e41444ccc1793c822694e11bfc3c2c4dff73e1776c524b0c394473fca0ee4`  
		Last Modified: Sat, 04 Feb 2023 13:28:24 GMT  
		Size: 4.4 MB (4416187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714a7ea9e9fbbb1b54589616d058bdaddf008e97dab522f0e8a8b4bf85f4c466`  
		Last Modified: Sat, 04 Feb 2023 13:28:23 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487612a90945fee63cb817b5b701744317b2bbb71de72f1455b73541c6ba9dcb`  
		Last Modified: Sat, 04 Feb 2023 13:28:23 GMT  
		Size: 1.4 MB (1403208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039cd64a8d6fc697c9499be365a437faac43b82ee3df2c7aca1ad2a7b6d608df`  
		Last Modified: Sat, 04 Feb 2023 13:28:22 GMT  
		Size: 8.0 MB (8045165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b00482c5d86ccea6a836605f9a1b7d43fd9ee06be0be3b13098e3ed62c5497`  
		Last Modified: Sat, 04 Feb 2023 13:28:21 GMT  
		Size: 1.2 MB (1249160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7413c2ab6643c2d5be9916b4830ee7ee9a839ec3b3ab62ef97d8a0f4b87d0eb8`  
		Last Modified: Sat, 04 Feb 2023 13:28:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209f1869e3afb49cd84436f8a8cfc67416ac6897750998bb73f1dbeaee48c443`  
		Last Modified: Sat, 04 Feb 2023 13:28:21 GMT  
		Size: 3.2 KB (3202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01ae8d06808c3ed3f9739ccebc613acfaaa6443cdafbfe3d790800b32a28767`  
		Last Modified: Sat, 04 Feb 2023 13:29:25 GMT  
		Size: 86.6 MB (86607149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70be5f83990065319c700ce91a254e360df3a0cf12dc3a2c708d00707324ce2c`  
		Last Modified: Sat, 04 Feb 2023 13:29:16 GMT  
		Size: 9.4 KB (9363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223ff3b4202cf48d4d3a3b8ef794afdab03695d8e5d8a5ddb47d5b015af91a18`  
		Last Modified: Sat, 04 Feb 2023 13:29:16 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f47e4425e6296511a127682010d40abf4abd9007765b9b001aed02a6424188`  
		Last Modified: Sat, 04 Feb 2023 13:29:16 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a30038dd9edd53757a7d2b47619f03a07feba202307c83d93c0e0161014cd6b`  
		Last Modified: Sat, 04 Feb 2023 13:29:16 GMT  
		Size: 4.8 KB (4780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:bb72f703a6a80958c68b8d06240a07f5ae132144f4f6668fa9d2b74e8e0457f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138303139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:461297ee90c3bc623e501969568c77660085df1833efa6e7a32a19a5223e1350`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 15:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 15:50:50 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 04 Feb 2023 15:50:51 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Feb 2023 15:51:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 04 Feb 2023 15:51:08 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 04 Feb 2023 15:51:09 GMT
ENV LANG=en_US.utf8
# Sat, 04 Feb 2023 15:51:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 15:51:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 04 Feb 2023 15:51:17 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 04 Feb 2023 16:18:54 GMT
ENV PG_MAJOR=13
# Sat, 04 Feb 2023 16:18:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Sat, 04 Feb 2023 16:18:56 GMT
ENV PG_VERSION=13.9-1.pgdg110+1
# Sat, 04 Feb 2023 16:31:30 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 16:31:31 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 16:31:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 16:31:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 16:31:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 16:31:35 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 16:31:37 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 16:31:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 16:31:38 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 16:31:39 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 16:31:40 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d5562e9108729c139eb383e4115735aba6ad598c8fa06979180d9026829d66`  
		Last Modified: Sat, 04 Feb 2023 16:58:45 GMT  
		Size: 4.6 MB (4607396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4adb8c7271ee68926c23f48a6b4e2da428541c992988b9033506a14667596d8`  
		Last Modified: Sat, 04 Feb 2023 16:58:43 GMT  
		Size: 1.6 KB (1639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1901d99798f1eca342d20c76078bc08e164ccbf96e931c132e5a5f3bd7d4de73`  
		Last Modified: Sat, 04 Feb 2023 16:58:43 GMT  
		Size: 1.4 MB (1446463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edb0ae75f911791beadf04785124e449b0f26301a53be52fcaed1f71ad5d031`  
		Last Modified: Sat, 04 Feb 2023 16:58:43 GMT  
		Size: 8.0 MB (8043333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347120c75ac26a044d443c46e5a5aaa024c9bcb6ed5072a01f3de2ecce76de8e`  
		Last Modified: Sat, 04 Feb 2023 16:58:42 GMT  
		Size: 1.0 MB (1027959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f0a2c440e0252704000f30eea5a3997c6a692309d6c653c8a353941424a201`  
		Last Modified: Sat, 04 Feb 2023 16:58:41 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467311549dffa7f2472aad4b7747ee89a72a99e2ff6af0dd918e098c6a16c44a`  
		Last Modified: Sat, 04 Feb 2023 16:58:41 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467109d43abb15a09490cb7b8b51a977015cebc354f282b17249d4cadf99b163`  
		Last Modified: Sat, 04 Feb 2023 17:00:06 GMT  
		Size: 90.8 MB (90782872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1556079d82f665d9b11cd9cc97431d3b226c770924ed1b5076562dd1430174e6`  
		Last Modified: Sat, 04 Feb 2023 16:59:53 GMT  
		Size: 9.4 KB (9362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8273521d398cccd9e204c70243467b13e9fe092e85c72b922d314a51060d9541`  
		Last Modified: Sat, 04 Feb 2023 16:59:54 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d48b4d1411c546a1426197f2f6834ab6686dc3452aef07e6aa1e13b143d08f2`  
		Last Modified: Sat, 04 Feb 2023 16:59:53 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6630f902a66c7daf61cda4a64007e95647cade7c4720576665be264b5dfc8bb`  
		Last Modified: Sat, 04 Feb 2023 16:59:53 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:3b241946c823c5489cede3a5ad09955f2a6bea6485ce73c98d00eb41595272fb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131095551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcc61315e377de1155fed560ee3bbc49f361e56e5335efce2e592595d79bba05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 04 Feb 2023 06:20:15 GMT
ADD file:03d6cf2d45a21e59975a1d17c6ca9fc83bb7a0da235873315c9c7940245beb1e in / 
# Sat, 04 Feb 2023 06:20:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 11:24:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 11:24:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 04 Feb 2023 11:24:36 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Feb 2023 11:25:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 04 Feb 2023 11:25:38 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 04 Feb 2023 11:25:40 GMT
ENV LANG=en_US.utf8
# Sat, 04 Feb 2023 11:25:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:26:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 04 Feb 2023 11:26:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 04 Feb 2023 13:28:14 GMT
ENV PG_MAJOR=13
# Sat, 04 Feb 2023 13:28:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Sat, 04 Feb 2023 13:28:19 GMT
ENV PG_VERSION=13.9-1.pgdg110+1
# Sat, 04 Feb 2023 14:25:15 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 14:25:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 14:25:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 14:25:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 14:25:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 14:25:40 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 14:25:42 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:25:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 14:25:49 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:25:53 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 14:25:56 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:aedd2a952aead0f89a308f23f44377263665bf76192d5542abd66473ea799d44`  
		Last Modified: Sat, 04 Feb 2023 06:28:25 GMT  
		Size: 29.6 MB (29619892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0563ff2a7376bd58df5a0d8093dbc2e3bffeae967406a030310572635689a0e5`  
		Last Modified: Sat, 04 Feb 2023 16:16:34 GMT  
		Size: 4.2 MB (4196257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce02eeaa75426698c696b6dabfed79f4275e8150b96fa3774a5962e72a3a1ca`  
		Last Modified: Sat, 04 Feb 2023 16:16:28 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bff052a7306d89ba1344b451f95617def7de3609c7e5425929a778dc725cf33`  
		Last Modified: Sat, 04 Feb 2023 16:16:30 GMT  
		Size: 1.4 MB (1358187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a12537cf5fa2e5906b6aa71aee12df4b287d64fcfbb184674a305f40a41806c`  
		Last Modified: Sat, 04 Feb 2023 16:16:34 GMT  
		Size: 8.0 MB (8043901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd02c90ca7e1eaaaa702370aa75417b717d85480622cb2ae394f75ef4ace0321`  
		Last Modified: Sat, 04 Feb 2023 16:16:27 GMT  
		Size: 1.1 MB (1089523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8225be314e3ccf262601382c1874bc44519601135c22fc7019e5dac929c35cb7`  
		Last Modified: Sat, 04 Feb 2023 16:16:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2546d28433ce76edeba75cdaae0529bf10b4feff8c6753916ed4543416898c19`  
		Last Modified: Sat, 04 Feb 2023 16:16:26 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be39dca5d86b441cff3edb101c9f129ce1dd96785cfc0e2d6406a6c85b40cd9d`  
		Last Modified: Sat, 04 Feb 2023 16:19:55 GMT  
		Size: 86.8 MB (86768438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affff561253b132ed36493730a966cdcdd359e18b0768dc2d2cf212ba1ceb1a7`  
		Last Modified: Sat, 04 Feb 2023 16:18:58 GMT  
		Size: 9.4 KB (9367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5adb8d9281e7651b30f95f0249c16bdacd00058aaeaa54ef013cb446335c58b`  
		Last Modified: Sat, 04 Feb 2023 16:18:58 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af9bc1867d3ed9d09ad4737ac0899605291bf9778b991dbe6746cc82019ffab`  
		Last Modified: Sat, 04 Feb 2023 16:18:58 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7c31aef0acb88201e892f70af12691307e0d0361c8a75e5e46c49ec21b9633`  
		Last Modified: Sat, 04 Feb 2023 16:18:58 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:4705cfff1c6a8d4bbf2b8366c1d807c72f9fa82d198c64e7b7cce03c5c0c132c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.7 MB (145691815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c767e7489b0a6db3ea53994e83632e7057413c9ca45ac812cdfbb86b8f599d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:19:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 18:19:30 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 04 Feb 2023 18:19:31 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Feb 2023 18:19:48 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 04 Feb 2023 18:20:02 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 04 Feb 2023 18:20:03 GMT
ENV LANG=en_US.utf8
# Sat, 04 Feb 2023 18:20:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:20:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 04 Feb 2023 18:20:16 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 04 Feb 2023 18:22:35 GMT
ENV PG_MAJOR=13
# Sat, 04 Feb 2023 18:22:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Sat, 04 Feb 2023 18:22:36 GMT
ENV PG_VERSION=13.9-1.pgdg110+1
# Sat, 04 Feb 2023 18:23:15 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 18:23:21 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 18:23:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 18:23:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 18:23:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 18:23:26 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 18:23:27 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 18:23:27 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 18:23:28 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 18:23:28 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147538f2b6f4fb300b3e6f3a212bfab4cc523da23c553528e6c2d113f7ba6d3d`  
		Last Modified: Sat, 04 Feb 2023 18:28:04 GMT  
		Size: 5.2 MB (5222816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dded9c3d7304c5207699460d3182a92f7050cf9bd64e0313be48b2ce52892be`  
		Last Modified: Sat, 04 Feb 2023 18:28:02 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68342fb671d1bdbfbb63233ebe4aeed0dd401c14cc754ceb3163cc7a6a2008b3`  
		Last Modified: Sat, 04 Feb 2023 18:28:03 GMT  
		Size: 1.4 MB (1393194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178a59fc05b566a526fa4283eb2d9a92c4b81eb3df33c51ac44adb37cd8bf0fd`  
		Last Modified: Sat, 04 Feb 2023 18:28:03 GMT  
		Size: 8.0 MB (8045226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb6462e2a28d0a0bb5b688c1fa30344a66b7d83a324f8d783a9e70db47f201a`  
		Last Modified: Sat, 04 Feb 2023 18:28:00 GMT  
		Size: 1.4 MB (1420126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae582f134adcd9c64826b10289aaf68d9ae7b4f5a7ad0454056bb2e92651b1bd`  
		Last Modified: Sat, 04 Feb 2023 18:28:00 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4fb1553b48511095a40dd5a7616cc2186bb6c329a12041e84fc71d6ddd9d49`  
		Last Modified: Sat, 04 Feb 2023 18:28:00 GMT  
		Size: 3.2 KB (3202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f95511ffe311549196680485619f72331ce12f791680fc78dc6704c1a281a0`  
		Last Modified: Sat, 04 Feb 2023 18:30:07 GMT  
		Size: 94.3 MB (94322037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5824b62b08fa9cbd26b5df839490a60c6b46949a8e0cd4a7b681b328bf97cec8`  
		Last Modified: Sat, 04 Feb 2023 18:29:42 GMT  
		Size: 9.4 KB (9360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5332617150bac3d0e704fdfd74561cecedfd5028ae642d0c6ed995663c633d`  
		Last Modified: Sat, 04 Feb 2023 18:29:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f02f29cb07b024633afd6ea1fc824d9672ee463af42ac989078e2c5a769dc8`  
		Last Modified: Sat, 04 Feb 2023 18:29:42 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e258ed43e0f49f2f038a62db44e6a6cb162097d3df753718561d45a80931dc5`  
		Last Modified: Sat, 04 Feb 2023 18:29:42 GMT  
		Size: 4.8 KB (4780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:6386810f8b0d64c246a7905aa1c2429ba22f13ac6fcfcdaadf958cc90c2a310a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140385117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98a0f9e2df7d523a70cb5e435ea2fbfc230445acfc3c499fa214959f8837c51d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:32:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 03:32:03 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 09 Feb 2023 03:32:03 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Feb 2023 03:32:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 09 Feb 2023 03:32:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 09 Feb 2023 03:32:15 GMT
ENV LANG=en_US.utf8
# Thu, 09 Feb 2023 03:32:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 03:32:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 09 Feb 2023 03:32:19 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 09 Feb 2023 03:46:27 GMT
ENV PG_MAJOR=13
# Thu, 09 Feb 2023 03:46:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Thu, 09 Feb 2023 03:46:27 GMT
ENV PG_VERSION=13.9-1.pgdg110+1
# Thu, 09 Feb 2023 03:55:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 09 Feb 2023 03:55:26 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 09 Feb 2023 03:55:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 09 Feb 2023 03:55:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Feb 2023 03:55:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 09 Feb 2023 03:55:27 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Feb 2023 03:55:27 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Thu, 09 Feb 2023 03:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 03:55:27 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 03:55:27 GMT
EXPOSE 5432
# Thu, 09 Feb 2023 03:55:28 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44696ba3a33f00900e18de97733d5e64b3a4e5c8d5dda5bc71c1af8c5bdbf82`  
		Last Modified: Thu, 09 Feb 2023 04:08:02 GMT  
		Size: 4.3 MB (4302266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2c50219e9cd684f91779c0eefd9b4d4e3ca0a1c304525b2843d984cea02cee`  
		Last Modified: Thu, 09 Feb 2023 04:08:01 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443a532a537ae78b9b3ee1f6e693d84fd32d8a7164c6b5e94ea9d09df805b9b3`  
		Last Modified: Thu, 09 Feb 2023 04:08:01 GMT  
		Size: 1.4 MB (1437003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1056003470c0a9ade00470b8d1773bb5d3e46962000687d2cdce0b3e7fe05`  
		Last Modified: Thu, 09 Feb 2023 04:08:01 GMT  
		Size: 8.1 MB (8099227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae22b3159dc9de8ee74eabbb25abc6bff4089bacaf4de4efb3072360e90ced46`  
		Last Modified: Thu, 09 Feb 2023 04:08:00 GMT  
		Size: 1.2 MB (1237938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a209d147d966142b7810dd8007b371f4555d95e512996f22b264ec9156bb0c23`  
		Last Modified: Thu, 09 Feb 2023 04:08:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ca0b46cbe800537be8001e255e52245cdc54d8ae7619df453abf8b39616cb6`  
		Last Modified: Thu, 09 Feb 2023 04:08:00 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c722ce02bf29e368981d02315c14e2892ba6354c17afd192405bdd5d63287b8`  
		Last Modified: Thu, 09 Feb 2023 04:08:56 GMT  
		Size: 95.6 MB (95641535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752fb8e19514826310661fc296e1bc1fcd6d15e0078dfb4d1160106be5bea1e2`  
		Last Modified: Thu, 09 Feb 2023 04:08:45 GMT  
		Size: 9.4 KB (9363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761b23f4c37e51534765fc639faf6655f49f4206d670f972e70020b104b043f`  
		Last Modified: Thu, 09 Feb 2023 04:08:45 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44df68351e4b15466638054a78cac7f40676f180709d6338c413984a7d9235e2`  
		Last Modified: Thu, 09 Feb 2023 04:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde0a725899a44c8c6c9137d601ed739b7212e95c9471200754f89da8445f554`  
		Last Modified: Thu, 09 Feb 2023 04:08:45 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
