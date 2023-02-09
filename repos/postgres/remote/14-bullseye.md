## `postgres:14-bullseye`

```console
$ docker pull postgres@sha256:150f7c41dfb6ae7465f35ece9fd77be09554ec8c9de3eed40c0ea9e069af6412
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

### `postgres:14-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:50befbf8d1901cc117a29a935a32f97b3a3c6d62bc93811123c63134e98f853c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137981306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d4e40f6b50987185528556a7adb03e8ef5b4ce6c21c4eef0030a025b46bdf4`
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
# Thu, 09 Feb 2023 04:40:32 GMT
ENV PG_MAJOR=14
# Thu, 09 Feb 2023 04:40:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 09 Feb 2023 04:40:32 GMT
ENV PG_VERSION=14.6-1.pgdg110+1
# Thu, 09 Feb 2023 04:40:50 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 09 Feb 2023 04:40:52 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 09 Feb 2023 04:40:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 09 Feb 2023 04:40:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Feb 2023 04:40:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 09 Feb 2023 04:40:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Feb 2023 04:40:53 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 04:40:53 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 04:40:53 GMT
EXPOSE 5432
# Thu, 09 Feb 2023 04:40:54 GMT
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
	-	`sha256:804b23d514380bfa87ac6ca37893de50284752fa385274688bafaf4281e578bf`  
		Last Modified: Thu, 09 Feb 2023 04:43:53 GMT  
		Size: 91.4 MB (91356916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d377381b80ae91d1391000b782ddfe27b96bf541a5a9eda24ff7f68ea3f843`  
		Last Modified: Thu, 09 Feb 2023 04:43:40 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdba78b944577797a79b2e3b70c85a6cce282793db0b45825d418c9de68608b`  
		Last Modified: Thu, 09 Feb 2023 04:43:40 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfca31b73d7d2c096296ae41f53de926f0fe8f7309b0ae254cc1c61474601104`  
		Last Modified: Thu, 09 Feb 2023 04:43:40 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587f867eece72f32c0c124584d6b49743407398b6391cb1e1310a8c36b64d5b`  
		Last Modified: Thu, 09 Feb 2023 04:43:40 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:1a5836054ab656d47452c95a8cbb3f3ae3a10b57f9d01e1d3ba68104e86f1235
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.3 MB (131251884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:984cabe96a9b47d28fb8ff6e32a1d3cf5cb322c031240c6a14e0ddfdacad763d`
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
# Thu, 09 Feb 2023 03:58:50 GMT
ENV PG_MAJOR=14
# Thu, 09 Feb 2023 03:58:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 09 Feb 2023 03:58:50 GMT
ENV PG_VERSION=14.6-1.pgdg110+1
# Thu, 09 Feb 2023 04:14:42 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 09 Feb 2023 04:14:43 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 09 Feb 2023 04:14:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 09 Feb 2023 04:14:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Feb 2023 04:14:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 09 Feb 2023 04:14:45 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Feb 2023 04:14:45 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Thu, 09 Feb 2023 04:14:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 04:14:45 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 04:14:45 GMT
EXPOSE 5432
# Thu, 09 Feb 2023 04:14:45 GMT
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
	-	`sha256:08956e10ce2964969a98ee935be0c4cec3924eb68ea611a50c6e56d212f96515`  
		Last Modified: Thu, 09 Feb 2023 05:01:52 GMT  
		Size: 87.5 MB (87468441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c19582607ecd22b3a86c0e8d14685d652deb94d038ea19c4fab6efaf219b1b6`  
		Last Modified: Thu, 09 Feb 2023 05:01:34 GMT  
		Size: 9.5 KB (9541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f654d3c57ee8f6c1ccc64e9604f7afd7241b80655afe7266145d5ffafd55733`  
		Last Modified: Thu, 09 Feb 2023 05:01:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a5a30d7a5402862d5335ab57f361f97ce4877e215e7c7a92e81655047edf4e`  
		Last Modified: Thu, 09 Feb 2023 05:01:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46140a0b1bdcad3179e76b285deab6955723e3954e87770962e08e57dab38452`  
		Last Modified: Thu, 09 Feb 2023 05:01:34 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:b94cdb84df26ce7a0b4af1568663e8d660bf249b908bac3134205c28f6d6bc7d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125887728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8f6ac2be0555e81fbbfa107c9423c97648edd64924663e250b1cc0183b48ab8`
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
# Sat, 04 Feb 2023 19:15:55 GMT
ENV PG_MAJOR=14
# Sat, 04 Feb 2023 19:15:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Sat, 04 Feb 2023 19:15:55 GMT
ENV PG_VERSION=14.6-1.pgdg110+1
# Sat, 04 Feb 2023 19:29:43 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 19:29:44 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 19:29:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 19:29:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 19:29:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 19:29:45 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 19:29:46 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 19:29:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 19:29:46 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 19:29:46 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 19:29:46 GMT
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
	-	`sha256:6f8288333b9c29020fb3158f4b1126cbffa13d44c3aa7f933d5a4b02864886a8`  
		Last Modified: Sat, 04 Feb 2023 20:12:23 GMT  
		Size: 85.0 MB (84976363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8964f6248e3be12fc01e55707c2479ddb09a002cf0ee7e41951ceb53e642c0`  
		Last Modified: Sat, 04 Feb 2023 20:12:08 GMT  
		Size: 9.5 KB (9537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d186700fc1185e37a932793b340c992d5bfea29dcade9eee97b0b9c6b5f90c3`  
		Last Modified: Sat, 04 Feb 2023 20:12:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86467bff050b5cbc10e2e92258c799f49477f0ee5d2d44cb9127744cdf5a4dad`  
		Last Modified: Sat, 04 Feb 2023 20:12:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a69bd4f2e38fe36b5dfba6558d75125c2a506076968497891721d3052ac16b4`  
		Last Modified: Sat, 04 Feb 2023 20:12:08 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:edca999f54c5666c9cecda32e36e16f16321a6dcb67da7c8833e7582deab1ca9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133058577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8965da136fb8c9feb9ec2031ea434a656f8fae2afb10a4a377c9541539944578`
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
# Sat, 04 Feb 2023 13:26:01 GMT
ENV PG_MAJOR=14
# Sat, 04 Feb 2023 13:26:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Sat, 04 Feb 2023 13:26:01 GMT
ENV PG_VERSION=14.6-1.pgdg110+1
# Sat, 04 Feb 2023 13:26:17 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 13:26:19 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 13:26:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 13:26:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 13:26:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 13:26:20 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 13:26:20 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:26:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 13:26:20 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 13:26:20 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 13:26:20 GMT
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
	-	`sha256:0cd13eeb7729db88ad7530b37ae5445f19152f3e44f1e6f96176ce2d17ca5b98`  
		Last Modified: Sat, 04 Feb 2023 13:29:00 GMT  
		Size: 87.9 MB (87880269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604fff3c78af362d0c74a8287f84c1527efffa4143bb139b76dc6f0f85ae0413`  
		Last Modified: Sat, 04 Feb 2023 13:28:51 GMT  
		Size: 9.5 KB (9538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7292c35063d90109ed7857cb125e07e20ffe13daa7e74cac83ea87dfd80e5579`  
		Last Modified: Sat, 04 Feb 2023 13:28:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5448d48757b249116f4ab6620fb4727771ba980fe00a627d1084e0b014d059`  
		Last Modified: Sat, 04 Feb 2023 13:28:51 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5b08e561735a2db8fb2a6f90bc1c418e1e2e5066795b7b6a4727ff73e33c0f`  
		Last Modified: Sat, 04 Feb 2023 13:28:51 GMT  
		Size: 4.8 KB (4777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:98ca6024e77894f584ce3dceeed3d14831af0e65ebaacec439cdbee2287ebe5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139586021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c980ec4ee124518d92feb24f75019ed7e75e6eb574c7d90fd973d76cbcd6980`
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
# Sat, 04 Feb 2023 16:05:19 GMT
ENV PG_MAJOR=14
# Sat, 04 Feb 2023 16:05:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Sat, 04 Feb 2023 16:05:21 GMT
ENV PG_VERSION=14.6-1.pgdg110+1
# Sat, 04 Feb 2023 16:18:31 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 16:18:31 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 16:18:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 16:18:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 16:18:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 16:18:35 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 16:18:37 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 16:18:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 16:18:38 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 16:18:39 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 16:18:40 GMT
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
	-	`sha256:a2b091cccd6ad9129ceab69d203dada58f8200797cb92b0813174866371626ef`  
		Last Modified: Sat, 04 Feb 2023 16:59:33 GMT  
		Size: 92.1 MB (92065577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199cd75c7071c2074c6495a1b06f8c34a52e446324b6d4652940b9c6b3b25402`  
		Last Modified: Sat, 04 Feb 2023 16:59:21 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319a17dc0a88677c51e523c445315be63621ec2e79b848f776fe2bbe8da2dafb`  
		Last Modified: Sat, 04 Feb 2023 16:59:21 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea501f6ac2c14aca9b3052166e69cbb717f9b1a7c57b72f1b9a6202a53ea4eb1`  
		Last Modified: Sat, 04 Feb 2023 16:59:21 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8977385e2ca513894ca7799939b22725ce68299fb03e9c9d9b3e9334280c5fd2`  
		Last Modified: Sat, 04 Feb 2023 16:59:21 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:641522ad1a8bb7db101ab5d88494fcdd164b6f19ea527c6b7695efcaf4e13d7b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.4 MB (132353941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:627ac5389bb9fec230b1ab601dc4f8f0ea4dd754cada049c6e5b236d98e4a53e`
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
# Sat, 04 Feb 2023 12:27:58 GMT
ENV PG_MAJOR=14
# Sat, 04 Feb 2023 12:28:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Sat, 04 Feb 2023 12:28:03 GMT
ENV PG_VERSION=14.6-1.pgdg110+1
# Sat, 04 Feb 2023 13:27:24 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 13:27:31 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 13:27:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 13:27:40 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 13:27:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 13:27:49 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 13:27:52 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:27:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 13:27:59 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 13:28:03 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 13:28:06 GMT
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
	-	`sha256:864c8a7d6213862769345157596644e340a9e102d79ff42c78665326e92a1755`  
		Last Modified: Sat, 04 Feb 2023 16:18:43 GMT  
		Size: 88.0 MB (88026653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab3db6f6dd3c89b0d42fa72a7cbdcc88678f6d9f4338acb84403fd0b6d1f243`  
		Last Modified: Sat, 04 Feb 2023 16:17:46 GMT  
		Size: 9.5 KB (9541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818e2bad18d0a66f5f537745bcccf705cfe092aade6b21383258aaee17b5a83`  
		Last Modified: Sat, 04 Feb 2023 16:17:46 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d951ea146bad0540e7a41c3da3b2f19e3a8abe1c042a1606c366d2e3384452`  
		Last Modified: Sat, 04 Feb 2023 16:17:46 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f0ef4c43a2f3e83cd44439cd7fc7c5a24c7748c2141664dc410de8ee78eeeb`  
		Last Modified: Sat, 04 Feb 2023 16:17:46 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:9771c1c347fb720ce9c28c807ed865b7410622ec2e6451324a8558a56cf4753a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147045887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7e799e31e83c5bf59df1f61f26dd6352e636b13db8e0f313b5acd17adb4ca1`
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
# Sat, 04 Feb 2023 18:21:29 GMT
ENV PG_MAJOR=14
# Sat, 04 Feb 2023 18:21:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Sat, 04 Feb 2023 18:21:30 GMT
ENV PG_VERSION=14.6-1.pgdg110+1
# Sat, 04 Feb 2023 18:22:12 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Feb 2023 18:22:17 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Feb 2023 18:22:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Feb 2023 18:22:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Feb 2023 18:22:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Feb 2023 18:22:21 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Feb 2023 18:22:21 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 18:22:22 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 18:22:22 GMT
EXPOSE 5432
# Sat, 04 Feb 2023 18:22:23 GMT
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
	-	`sha256:e9c540420616da0329829b4c2db6ffec41a67ffa42fda070cf982a994a268bbb`  
		Last Modified: Sat, 04 Feb 2023 18:29:20 GMT  
		Size: 95.7 MB (95675940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be947df0db9cfd943eac344b58df08f1f9f32b639805a588813ec83caf93865`  
		Last Modified: Sat, 04 Feb 2023 18:28:54 GMT  
		Size: 9.5 KB (9533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c6a4e27fecdff07b11ce061a609458a850ee8bd146800f75483596efebef3b`  
		Last Modified: Sat, 04 Feb 2023 18:28:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcfbfb203c36a387545ccaac15d17b031e0d220366107849037f59006a31858`  
		Last Modified: Sat, 04 Feb 2023 18:28:55 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbcb6cafd9918a9f507ae78446d3426036276ad3f8b6d3e15ee8a07b27d7d55`  
		Last Modified: Sat, 04 Feb 2023 18:28:54 GMT  
		Size: 4.8 KB (4778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:7e15ddb54749ac813a2449b06bf8ed0dc0d172810b1bf112b976aad01e8c7b3b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.2 MB (85229163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b219890cd5e99aa44d5ac6dac34805c63f7ab0eed2cf45e4be95f8875e461020`
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
# Thu, 09 Feb 2023 03:39:28 GMT
ENV PG_MAJOR=14
# Thu, 09 Feb 2023 03:39:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 09 Feb 2023 03:39:28 GMT
ENV PG_VERSION=14.6-1.pgdg110+1
# Thu, 09 Feb 2023 03:46:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 09 Feb 2023 03:46:12 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 09 Feb 2023 03:46:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 09 Feb 2023 03:46:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Feb 2023 03:46:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 09 Feb 2023 03:46:13 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Feb 2023 03:46:13 GMT
COPY file:d4c2ceee202d1390df115217c6e567abc1da7a31572f20a840d966332148ebe4 in /usr/local/bin/ 
# Thu, 09 Feb 2023 03:46:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 03:46:13 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 03:46:13 GMT
EXPOSE 5432
# Thu, 09 Feb 2023 03:46:14 GMT
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
	-	`sha256:5f48edcf7df2a48f394ffab76cb2a8ef01033535e5034951d0c09483912f7b71`  
		Last Modified: Thu, 09 Feb 2023 04:08:30 GMT  
		Size: 40.5 MB (40485400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ec32ccc2176fd6d21f7f53fbbb46cb00c4fd23c5973a58119b0a53f0fa735`  
		Last Modified: Thu, 09 Feb 2023 04:08:24 GMT  
		Size: 9.5 KB (9542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61640730d8c831c80ca38903bc4ec23d049e3156972f30463fcee1d31f3fa468`  
		Last Modified: Thu, 09 Feb 2023 04:08:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4380b0f852786ba88840818a57ede88463c3a6eecb43a592e70289a70c4fd9dd`  
		Last Modified: Thu, 09 Feb 2023 04:08:24 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d1e48fca7522d408a8a68172cfa07a6867b3a375a0d32b262ff99a353149d`  
		Last Modified: Thu, 09 Feb 2023 04:08:24 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
