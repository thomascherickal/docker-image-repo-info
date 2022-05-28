## `postgres:10-stretch`

```console
$ docker pull postgres@sha256:401f390c9db1b95109ff6a5476096ad7f222c469862eaf2e82a2af34f5f010b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:10-stretch` - linux; amd64

```console
$ docker pull postgres@sha256:29e643048dc946894eca94d2eab2c1f9a2e939e0661294ad7f44c3253a5c6fd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74101910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e72caba743b561cec2e1889ae3c80ff3d126aa720748ea797bb06736cab17f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 11 May 2022 01:22:15 GMT
ADD file:026b786cdb9bd5132e483b55e6486a88dc97cd0f1dca7a128c56975e912865c3 in / 
# Wed, 11 May 2022 01:22:15 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:24:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 12:24:15 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 11 May 2022 12:24:15 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 12:24:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 12:24:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 11 May 2022 12:24:33 GMT
ENV LANG=en_US.utf8
# Wed, 11 May 2022 12:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:24:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 12:24:40 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 12:25:29 GMT
ENV PG_MAJOR=10
# Wed, 11 May 2022 12:25:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 18 May 2022 00:51:41 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Wed, 18 May 2022 00:51:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 18 May 2022 00:51:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 18 May 2022 00:51:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 18 May 2022 00:51:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 18 May 2022 00:51:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 18 May 2022 00:51:57 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 18 May 2022 00:51:57 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 18 May 2022 00:51:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 18 May 2022 00:51:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 May 2022 00:51:57 GMT
STOPSIGNAL SIGINT
# Wed, 18 May 2022 00:51:57 GMT
EXPOSE 5432
# Wed, 18 May 2022 00:51:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d956d1d1888bd62aafc454609f2d7adc3a3ee5f9678bb80e4d9d27662c230884`  
		Last Modified: Wed, 11 May 2022 01:28:58 GMT  
		Size: 22.6 MB (22567372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d38a6d6dc2cf97b12bd91608ffbf5981803dfafad39a1cbb346fb5675aea8a5`  
		Last Modified: Wed, 11 May 2022 12:28:42 GMT  
		Size: 4.5 MB (4504008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be54560233f231fd4ac3e3f885899b0f98e1b3ef261e6d477c8b61569d1cc1e1`  
		Last Modified: Wed, 11 May 2022 12:28:40 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4d732b0710d28b3fb805d35cb3cb5d1efae28629b501600f0bd52212a72529`  
		Last Modified: Wed, 11 May 2022 12:28:41 GMT  
		Size: 1.4 MB (1379570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800077ca5ad1e65115b5feaf027255ae94411609cca53cc68df65d1856c73727`  
		Last Modified: Wed, 11 May 2022 12:28:39 GMT  
		Size: 6.2 MB (6185777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25ba21882ce5604cbc677fe2379cf892f9c4dfd35633c14edff5fdf05355363`  
		Last Modified: Wed, 11 May 2022 12:28:39 GMT  
		Size: 1.2 MB (1249933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d179a9f8acc69c51af21fa075876049cdd1f2ee90545926fd157251c9c8c7e7a`  
		Last Modified: Wed, 11 May 2022 12:28:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a607a1546a23fdc5d322003f62c0fac0f6e8ff30081cb8edda271617d4bacf8`  
		Last Modified: Wed, 11 May 2022 12:28:38 GMT  
		Size: 5.6 KB (5578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350896fc407f37e2cf792e9fc9567e93b1f4d89488e03f9e3feb0e6fbd2af67a`  
		Last Modified: Wed, 18 May 2022 01:00:46 GMT  
		Size: 38.2 MB (38194494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cfdc68db7617084b59ee4b2f64f2a31f70b0e87fa6ce4300c1408ff1bd1ffbd`  
		Last Modified: Wed, 18 May 2022 01:00:38 GMT  
		Size: 8.1 KB (8070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d437cbce7acd4309d98e23af06377952e804a40190bb0e2178b4ac7f6dd6e8e`  
		Last Modified: Wed, 18 May 2022 01:00:39 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1f8a3b63b4fd77ff4fdda94eee6083cd303da504e1e9d25aaeb84f46515d83`  
		Last Modified: Wed, 18 May 2022 01:00:38 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3545013681b0a0cb174961e6c13589a2646a91c2b6534e6b3d12f4b69ae8a76f`  
		Last Modified: Wed, 18 May 2022 01:00:38 GMT  
		Size: 4.7 KB (4706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96575b202bd527664476be0b1c2878787ddab7266d776f93f0fa8017f4fe71dd`  
		Last Modified: Wed, 18 May 2022 01:00:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:f071c2514359ec22f7b8fa7b4daab3bed7e1c490c22cb80e7af6e61089ca7642
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71089819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f3d3320330cb68203368f1819eb5d034d767eb8e435e4987dbd8c4d82e3cb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 11 May 2022 00:56:06 GMT
ADD file:efd3ed6309109e633b701403f7004b3b175b74971a18b46b1d481f075dd5c8f5 in / 
# Wed, 11 May 2022 00:56:06 GMT
CMD ["bash"]
# Wed, 11 May 2022 22:33:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 22:33:21 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 11 May 2022 22:33:22 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 22:33:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 22:34:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 11 May 2022 22:34:14 GMT
ENV LANG=en_US.utf8
# Wed, 11 May 2022 22:34:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 22:34:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 22:34:33 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 23:25:19 GMT
ENV PG_MAJOR=10
# Wed, 11 May 2022 23:25:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 18 May 2022 04:20:02 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Wed, 18 May 2022 04:46:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 18 May 2022 04:46:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 18 May 2022 04:46:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 18 May 2022 04:46:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 18 May 2022 04:46:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 18 May 2022 04:46:27 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 18 May 2022 04:46:27 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 18 May 2022 04:46:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 18 May 2022 04:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 May 2022 04:46:29 GMT
STOPSIGNAL SIGINT
# Wed, 18 May 2022 04:46:30 GMT
EXPOSE 5432
# Wed, 18 May 2022 04:46:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cf06fd8914d4c16f6407e9b08c3fb21faf74781e70c848c5994854f41d186ade`  
		Last Modified: Wed, 11 May 2022 01:13:42 GMT  
		Size: 21.2 MB (21240674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2914c114ab9c321a27e1fa57202badc92bcce7b8df0881d2c05164879e00911e`  
		Last Modified: Wed, 11 May 2022 23:59:00 GMT  
		Size: 4.2 MB (4239521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a6964d4ac9093ebec3d435cef74361473ae4255edf496ddeb08d71c4642d23`  
		Last Modified: Wed, 11 May 2022 23:58:57 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be121304dd7931d8a2e034e5076e57f64f0f791cdc0b67ced08933e1441b919d`  
		Last Modified: Wed, 11 May 2022 23:58:58 GMT  
		Size: 1.3 MB (1344488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e6d98a8f348c427aff6067c94b66cd159d4f972aca6c73fec0ab01eb265c90`  
		Last Modified: Wed, 11 May 2022 23:59:01 GMT  
		Size: 6.2 MB (6185881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2b531a132f0a00889204721f01e72ef30b00ef0fa665e472b699083d2fdc46`  
		Last Modified: Wed, 11 May 2022 23:58:56 GMT  
		Size: 1.2 MB (1194897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715ebfd372c8ce71471b1febf5c0b856a07096e57e79ce00071c7238b8972449`  
		Last Modified: Wed, 11 May 2022 23:58:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a3517ba6fe10086449e5141940c07640d873a7e85c91c5991452dacb8f64ea`  
		Last Modified: Wed, 11 May 2022 23:58:55 GMT  
		Size: 5.6 KB (5583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f0a07cf074f798c38cc3c55101251c3103dee383ff110faf083e9495b9c3a0`  
		Last Modified: Wed, 18 May 2022 04:55:39 GMT  
		Size: 36.9 MB (36863598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43ab5cc166512b6169e1f7441d5849ac5b87e6b3bf7d60af2c397d3f5ba49c6`  
		Last Modified: Wed, 18 May 2022 04:55:11 GMT  
		Size: 8.1 KB (8076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffce54af450655c11f3bfaa4f880225d92259ffd67a815010433d562b6f990f0`  
		Last Modified: Wed, 18 May 2022 04:55:11 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed56ae33589be2a3e58574d74840d169c70b04110480487d2a68cfb5d4f588a`  
		Last Modified: Wed, 18 May 2022 04:55:11 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ed2b92772873d229af7adf91221466093b498462c28033c161d3f04483ebf7`  
		Last Modified: Wed, 18 May 2022 04:55:12 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4475a7a80bc7f84714fffaa7f46cc646e54719829867cfb138ddb2e4eac20468`  
		Last Modified: Wed, 18 May 2022 04:55:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:f7b5920b581cb95c7419eea0dc94e29c59685e3116fa3e33bd7580a4264a735a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67681329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d919cdf70aa2d6d44585144f3d5a37ebff5fd9702467851058a5c026fea741b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 11 May 2022 01:55:08 GMT
ADD file:2053868b10dc5164f3fb9b77a89aafd3da73e08ef244700b78666cc3e0f05b0f in / 
# Wed, 11 May 2022 01:55:09 GMT
CMD ["bash"]
# Wed, 11 May 2022 20:15:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 20:15:57 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 11 May 2022 20:15:57 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 20:16:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 20:16:43 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 11 May 2022 20:16:44 GMT
ENV LANG=en_US.utf8
# Wed, 11 May 2022 20:16:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 20:16:55 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 20:16:59 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 21:03:20 GMT
ENV PG_MAJOR=10
# Wed, 11 May 2022 21:03:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 18 May 2022 05:03:13 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Wed, 18 May 2022 05:26:19 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 18 May 2022 05:26:21 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 18 May 2022 05:26:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 18 May 2022 05:26:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 18 May 2022 05:26:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 18 May 2022 05:26:25 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 18 May 2022 05:26:25 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 18 May 2022 05:26:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 18 May 2022 05:26:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 May 2022 05:26:28 GMT
STOPSIGNAL SIGINT
# Wed, 18 May 2022 05:26:28 GMT
EXPOSE 5432
# Wed, 18 May 2022 05:26:29 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1b0318fd9d43e032add67ea408393c8e890c1ea4b437ecc600ea0107fa7de956`  
		Last Modified: Wed, 11 May 2022 02:11:56 GMT  
		Size: 19.4 MB (19359811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53046a866d15d4760eb4e4d14f27c1b78e934c27cdf23944451d04b2d5d472b`  
		Last Modified: Wed, 11 May 2022 21:35:48 GMT  
		Size: 3.9 MB (3875769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e46571f7c56a215c3c363ec526c456f0ad61f9eaa4d9c41c12ee81a04592f6`  
		Last Modified: Wed, 11 May 2022 21:35:45 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a019daa04d80334befd97fa82686e0e9df2676870c278d4b332246d8dad00e`  
		Last Modified: Wed, 11 May 2022 21:35:46 GMT  
		Size: 1.3 MB (1336149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3985436eaeb41f1e25c39ae7b9462582d4df1999fe5b744a692ff35e1559a19f`  
		Last Modified: Wed, 11 May 2022 21:35:48 GMT  
		Size: 6.2 MB (6185636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360adf5f64b18d48c2fbe179ef1e2e386824648a294bbeb4ac3f6721e33785de`  
		Last Modified: Wed, 11 May 2022 21:35:44 GMT  
		Size: 1.1 MB (1097138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1dc6d892dfb74ff216fc1576534d368daf3cadd4b74d601b039547c8c5d19f`  
		Last Modified: Wed, 11 May 2022 21:35:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb68343b7b2e633a105703194198bf67e264972a9a759b5f40c2ec7ba3162bd`  
		Last Modified: Wed, 11 May 2022 21:35:44 GMT  
		Size: 5.6 KB (5583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a5b76b745537a5cd044ebb0c7d9782b9a93efbfc6e81904de6103499e5b0e8`  
		Last Modified: Wed, 18 May 2022 05:44:51 GMT  
		Size: 35.8 MB (35806064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d850ae3ea7f5c4a30d20d161bcd02e08b0f98f6027e9c9ffc2fbd136072ac54`  
		Last Modified: Wed, 18 May 2022 05:44:28 GMT  
		Size: 8.1 KB (8075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2a3939e477dca67aa653a333069013f09c00cc19c4341b7b943dcfd4a26813`  
		Last Modified: Wed, 18 May 2022 05:44:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309a7a3e3504fd2e66fcc66a278100c4c01e4813b98acef533a61e2f71c613fb`  
		Last Modified: Wed, 18 May 2022 05:44:29 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb1e656bb49a164ca6928cf56507149add89b3dead89e39ab7ed136f2a8126c`  
		Last Modified: Wed, 18 May 2022 05:44:29 GMT  
		Size: 4.7 KB (4707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3df531914fbd569f031a5aab030f615051384964a1ccc99f172afe833b5a22`  
		Last Modified: Wed, 18 May 2022 05:44:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:826e136b95290848c7cff8e3fd2d7642278f5fe76f11c09db178b5d366ac4890
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (69985590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f579ed3acd9b4991e97c2f8e74feccd551a2c38516dea599781408b1baecb938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 28 May 2022 00:43:00 GMT
ADD file:5d3acfb1c09652c954868b7e7fba2e995e5e143bd0f2b1c04a34897232913f7a in / 
# Sat, 28 May 2022 00:43:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 06:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 06:50:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 28 May 2022 06:50:54 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 06:51:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 06:51:12 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 28 May 2022 06:51:13 GMT
ENV LANG=en_US.utf8
# Sat, 28 May 2022 06:51:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 06:51:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 06:51:23 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 07:01:44 GMT
ENV PG_MAJOR=10
# Sat, 28 May 2022 07:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sat, 28 May 2022 07:01:46 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Sat, 28 May 2022 07:11:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 28 May 2022 07:11:24 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 28 May 2022 07:11:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 May 2022 07:11:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 May 2022 07:11:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 May 2022 07:11:27 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 May 2022 07:11:29 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Sat, 28 May 2022 07:11:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 28 May 2022 07:11:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 07:11:31 GMT
STOPSIGNAL SIGINT
# Sat, 28 May 2022 07:11:32 GMT
EXPOSE 5432
# Sat, 28 May 2022 07:11:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5787d8ce843947b58d50c514418ca92eca29e2110be4fe2993451d835d2d846a`  
		Last Modified: Sat, 28 May 2022 00:51:48 GMT  
		Size: 20.4 MB (20424104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17ea5d1e741473a39b1a7e5eca5a742b930d73b147217ddaa7bbe347e4aaca`  
		Last Modified: Sat, 28 May 2022 07:16:07 GMT  
		Size: 3.9 MB (3890932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497e293642c352f67b7637126f4eea8b184eb608cf50d376d8a2985c853980d`  
		Last Modified: Sat, 28 May 2022 07:16:06 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e99dbea293843ebcdf20ea4843c630325366f7f864665a3d1b71234b6f7a9a`  
		Last Modified: Sat, 28 May 2022 07:16:06 GMT  
		Size: 1.3 MB (1307859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09579ff3ea4da0bf8dd6881242db63a6eddf4994c794b4fa8cb07b22cb8ed281`  
		Last Modified: Sat, 28 May 2022 07:16:05 GMT  
		Size: 6.2 MB (6182574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dac6704479db1d6858a29da897365a51f12e23c655fdf8c3528db64a4dc270`  
		Last Modified: Sat, 28 May 2022 07:16:04 GMT  
		Size: 1.0 MB (1007478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9db756532cf3958282c4f6c52e9f0d8cc19a4ecda8d91ed30b3005744fb8473`  
		Last Modified: Sat, 28 May 2022 07:16:03 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed841cf8dfd2b92969f717e0e33d51f953a8837187b05edbb84312ebe6ecd43`  
		Last Modified: Sat, 28 May 2022 07:16:03 GMT  
		Size: 5.5 KB (5525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8aba4bb7a7c6f33554488852d50dad4a4eb67eabd0b3be89bd7c4b0c22de8d0`  
		Last Modified: Sat, 28 May 2022 07:16:57 GMT  
		Size: 37.2 MB (37152139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02222bad3091c57650545e3dc81b6278ea40feb146ce6e58bacad6ae80935c`  
		Last Modified: Sat, 28 May 2022 07:16:49 GMT  
		Size: 8.1 KB (8077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3735a732b755c42ef4f5c228062ad83affa852677a047ef706286c947d2aee`  
		Last Modified: Sat, 28 May 2022 07:16:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358615225b5b9c85c94a2d9efb4689a96fd75edca8c26590390fa55e0819009e`  
		Last Modified: Sat, 28 May 2022 07:16:49 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3a7c3c02f5fd24737a5cc2d864cc0e2a3b34d1791fbba4733780d0c7480988`  
		Last Modified: Sat, 28 May 2022 07:16:49 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ba9d5e8d445b554b2f0447dcc6f23720ab665909191d11e8238ade58581116`  
		Last Modified: Sat, 28 May 2022 07:16:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; 386

```console
$ docker pull postgres@sha256:7802ae6c410c15221925db5dc188c28d8ba35450a3b926b5b5a7ee7604167647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74852532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff9a3ce9417eb170ac2a8f6f1b01d6c1c81f4f4cb094a606a90ca2cabb972df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 11 May 2022 01:41:44 GMT
ADD file:99bd3f1842fa0bf09a3c19b09bb2291aeaa26ba30f2704a7074d1e9c395e1bbb in / 
# Wed, 11 May 2022 01:41:45 GMT
CMD ["bash"]
# Wed, 11 May 2022 10:25:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 10:25:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 11 May 2022 10:25:12 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 10:25:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 10:25:30 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 11 May 2022 10:25:31 GMT
ENV LANG=en_US.utf8
# Wed, 11 May 2022 10:25:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:25:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 10:25:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 10:35:36 GMT
ENV PG_MAJOR=10
# Wed, 11 May 2022 10:35:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 18 May 2022 02:10:14 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Wed, 18 May 2022 02:10:34 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 18 May 2022 02:10:35 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 18 May 2022 02:10:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 18 May 2022 02:10:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 18 May 2022 02:10:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 18 May 2022 02:10:39 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 18 May 2022 02:10:41 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 18 May 2022 02:10:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 18 May 2022 02:10:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 May 2022 02:10:43 GMT
STOPSIGNAL SIGINT
# Wed, 18 May 2022 02:10:44 GMT
EXPOSE 5432
# Wed, 18 May 2022 02:10:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5d986b441a1343c1b3027f0fcd148ee0392ceb52fd4b1e8cfb0de32bd1f09938`  
		Last Modified: Wed, 11 May 2022 01:50:52 GMT  
		Size: 23.2 MB (23202360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2925ddaf5865bac82afd07560a9d73e804c381fcdb1e4fb8888e62c70fbc3b5`  
		Last Modified: Wed, 11 May 2022 10:39:34 GMT  
		Size: 4.6 MB (4623951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba85d252d8ec188f1813e53d252a519f99c808a3dc911f1d05637210f2de275b`  
		Last Modified: Wed, 11 May 2022 10:39:33 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040a84a65089a783b9cac1f0c73d7c2c6044b4a7e161fcca3e278f83763a615`  
		Last Modified: Wed, 11 May 2022 10:39:33 GMT  
		Size: 1.3 MB (1346969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9961ee93ed5243457f2054aa9a244e64bc881a2b17e60a8b5dfd116d577ba56`  
		Last Modified: Wed, 11 May 2022 10:39:32 GMT  
		Size: 6.2 MB (6182820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33333f21d0b5aafa403ef8c1ce7e2e00bd651a8cf2533061f1e1215b65d5e4f`  
		Last Modified: Wed, 11 May 2022 10:39:31 GMT  
		Size: 1.0 MB (1030547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baae5be6dc2679245333b19d711f0252556d81233a753efc50c5bbbd9599664`  
		Last Modified: Wed, 11 May 2022 10:39:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b9314e82cf0cb8daeeb233b2bc86ca21c93af5c4d8ff706964a9760de3bbb`  
		Last Modified: Wed, 11 May 2022 10:39:30 GMT  
		Size: 5.5 KB (5527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bed3b1c8aef05c021bd8f2040610dfe847e03d13e130f5d26a2673568dde4b`  
		Last Modified: Wed, 18 May 2022 02:20:21 GMT  
		Size: 38.4 MB (38445391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d728afe6db0ed004b1f9a3a498a59a3c9d461de908857d546cd31ab85fcb55`  
		Last Modified: Wed, 18 May 2022 02:20:12 GMT  
		Size: 8.1 KB (8073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07df1e68e9387a35ffad053b54e3d0ae87f2b79d824b51f0693873b883f2c050`  
		Last Modified: Wed, 18 May 2022 02:20:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f69fa025a4e24d258281e24215e3ed1232f6a1e5f095d89e66856f7621cb7c4`  
		Last Modified: Wed, 18 May 2022 02:20:13 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db09dbd90cb0effb7cf9e7953d7f1b84cc73f0655b72210aba397fff4f6e753`  
		Last Modified: Wed, 18 May 2022 02:20:14 GMT  
		Size: 4.7 KB (4707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5333f4ad96f658116b2e9f5190e61573ea1639b49e87993e9aa7ccef9b66440d`  
		Last Modified: Wed, 18 May 2022 02:20:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
