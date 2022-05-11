## `postgres:10-stretch`

```console
$ docker pull postgres@sha256:e5eca94434d8e2c5a9e8efd23cac6fa7b243ee085ef16177f2db5004ceb54610
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
$ docker pull postgres@sha256:5e2c4d59cf599b1ca340713348c4af1c77f48b2b1c5a21358a94ba70ea00d167
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74096185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce853fb20ebfe60d79e8a29b80733a38639813f6182655ba64282e6e60db763f`
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
# Wed, 11 May 2022 12:25:29 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Wed, 11 May 2022 12:25:42 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 11 May 2022 12:25:43 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 11 May 2022 12:25:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 11 May 2022 12:25:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 11 May 2022 12:25:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 11 May 2022 12:25:44 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 11 May 2022 12:25:45 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 11 May 2022 12:25:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 May 2022 12:25:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 12:25:45 GMT
STOPSIGNAL SIGINT
# Wed, 11 May 2022 12:25:45 GMT
EXPOSE 5432
# Wed, 11 May 2022 12:25:45 GMT
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
	-	`sha256:53d725e43fc62bf5a0a17a04f2b83b56c934dcbb63d0369cf729b87960555684`  
		Last Modified: Wed, 11 May 2022 12:29:31 GMT  
		Size: 38.2 MB (38188764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df67bb4a94144299540f662eed0a6f20e707872128b5ebad2b11af3f2703a75`  
		Last Modified: Wed, 11 May 2022 12:29:23 GMT  
		Size: 8.1 KB (8073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e54f7c21f85e95699ebbfb37d23c197d6c757c5c5abe7e03d47a65d22fa2e04`  
		Last Modified: Wed, 11 May 2022 12:29:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea6cd75b42bcf5484fa3b93fd0578e02fcaca4b30a9682a20f076109b91c839`  
		Last Modified: Wed, 11 May 2022 12:29:23 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554cde7c53d5998bd45510c828e003c2b73ba38f8774abca99e93fcd67519151`  
		Last Modified: Wed, 11 May 2022 12:29:22 GMT  
		Size: 4.7 KB (4706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd331d4b9709a6d4bdb4afd0cef5f3cdb328e85ec5266706be78ac6a3284eff`  
		Last Modified: Wed, 11 May 2022 12:29:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:5eb23ca0ccc51a81620bec4cf33b3a862d26ee8e963e4e5e0f2d9474a626576c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71082747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb0836ea532519d2d4d8774a382943e712be0eb76f7f5b1dc075892b1e91eecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 07:22:40 GMT
ADD file:8caa5e7ca2ab4b420bed155bd2190baa73ca3c4e9378db02b0c0cede15974d69 in / 
# Wed, 20 Apr 2022 07:22:41 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 05:04:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Apr 2022 05:04:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 21 Apr 2022 05:04:53 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Apr 2022 05:05:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Apr 2022 05:05:45 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 21 Apr 2022 05:05:45 GMT
ENV LANG=en_US.utf8
# Thu, 21 Apr 2022 05:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 05:05:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Apr 2022 05:06:03 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 21 Apr 2022 05:57:03 GMT
ENV PG_MAJOR=10
# Thu, 21 Apr 2022 05:57:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Thu, 21 Apr 2022 05:57:04 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Thu, 21 Apr 2022 06:23:04 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 21 Apr 2022 06:23:06 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 21 Apr 2022 06:23:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 21 Apr 2022 06:23:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 21 Apr 2022 06:23:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 21 Apr 2022 06:23:10 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 21 Apr 2022 06:23:10 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Thu, 21 Apr 2022 06:23:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Apr 2022 06:23:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 06:23:13 GMT
STOPSIGNAL SIGINT
# Thu, 21 Apr 2022 06:23:13 GMT
EXPOSE 5432
# Thu, 21 Apr 2022 06:23:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2d96febf107fb8f8f8c5d8bd55514488bd2c5f9ca3c49cb1c015381d7aa816d6`  
		Last Modified: Wed, 20 Apr 2022 07:40:19 GMT  
		Size: 21.2 MB (21240552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9cd0b388029fbfa4d57c2ae64305c0a8c85323cf5385fef637d22359b031b0`  
		Last Modified: Thu, 21 Apr 2022 06:30:36 GMT  
		Size: 4.2 MB (4239488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d781ed8c92f5a9788a3d47a2251d2f520a385d125635abc18e10a98ef9addf2f`  
		Last Modified: Thu, 21 Apr 2022 06:30:33 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bcb22951ec385fe3134b67da8c047efec0cebb84e85b00ac03ab3b1adb0471`  
		Last Modified: Thu, 21 Apr 2022 06:30:34 GMT  
		Size: 1.3 MB (1344469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e581a6b855f249872175b1cb60b7e3bba40c4856d9b59921c8bfd667c741db3b`  
		Last Modified: Thu, 21 Apr 2022 06:30:35 GMT  
		Size: 6.2 MB (6185799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4479ef4ec7ac6d1caa391282c84b04a842084fd150f26cf3d4e960ed1de5bed6`  
		Last Modified: Thu, 21 Apr 2022 06:30:32 GMT  
		Size: 1.2 MB (1194860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b314b61736c98f0f1494aa7ef45e038647271883795f2e42fbd812aa8901ee1`  
		Last Modified: Thu, 21 Apr 2022 06:30:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55aed70ec75a7cee1628c53e6263cacd11e9ae72c08c8e9e4a5800a290153f06`  
		Last Modified: Thu, 21 Apr 2022 06:30:31 GMT  
		Size: 5.6 KB (5585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b97344b766875db8f4a6a499d79ae50e1ade194df2e0619dfd2fcbbc9a31ae`  
		Last Modified: Thu, 21 Apr 2022 06:32:25 GMT  
		Size: 36.9 MB (36856811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a85909cbbf9fc4bc8b7be7c22427cad50dcc5751b03890db6b91a2025b74e`  
		Last Modified: Thu, 21 Apr 2022 06:31:57 GMT  
		Size: 8.1 KB (8082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d771eb4c5de0153f373fbe04e56514a5494705139908138a64cf2312853cc6`  
		Last Modified: Thu, 21 Apr 2022 06:31:57 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dad485e54fa6cbd6fab5fd88bde45a8ad5088b1797676f54e288063803993d`  
		Last Modified: Thu, 21 Apr 2022 06:31:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc04577d2d129a07e138392bdcb05877ce0822903299422da09b6b717509ecf`  
		Last Modified: Thu, 21 Apr 2022 06:31:57 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069dd7b5c4a4f433f8ef852e76effb740285b468d46c32b7a95a18e2b92ce69b`  
		Last Modified: Thu, 21 Apr 2022 06:31:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:24ab1b5e609740fd5b932c6565c8b8be5efc1ebdd7e60bd1f67d3a150f048561
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67673330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a4db152032311bbe28d71544af3dc42bdb6bba973fadb41211cff7d7663dfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 13:33:51 GMT
ADD file:096692331564a30a9a9c6b24e681d99d68b54eeeabb7c5ac7d4073de06e050b2 in / 
# Wed, 20 Apr 2022 13:33:51 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 08:36:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Apr 2022 08:36:13 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 21 Apr 2022 08:36:14 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Apr 2022 08:36:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Apr 2022 08:37:00 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 21 Apr 2022 08:37:01 GMT
ENV LANG=en_US.utf8
# Thu, 21 Apr 2022 08:37:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 08:37:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Apr 2022 08:37:16 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 21 Apr 2022 09:23:17 GMT
ENV PG_MAJOR=10
# Thu, 21 Apr 2022 09:23:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Thu, 21 Apr 2022 09:23:18 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Thu, 21 Apr 2022 09:46:12 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 21 Apr 2022 09:46:15 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 21 Apr 2022 09:46:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 21 Apr 2022 09:46:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 21 Apr 2022 09:46:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 21 Apr 2022 09:46:20 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 21 Apr 2022 09:46:20 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Thu, 21 Apr 2022 09:46:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 21 Apr 2022 09:46:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 09:46:23 GMT
STOPSIGNAL SIGINT
# Thu, 21 Apr 2022 09:46:23 GMT
EXPOSE 5432
# Thu, 21 Apr 2022 09:46:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:08da560f0b65b004ba95f9a431d3ac51b8807b16ec6ef170e2e00dc55330246d`  
		Last Modified: Wed, 20 Apr 2022 13:51:07 GMT  
		Size: 19.4 MB (19359807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b330e9f5f7b6093bd31383fc931a0fa0a7eb6042397b6e3dcc03bb15cea72`  
		Last Modified: Thu, 21 Apr 2022 09:55:38 GMT  
		Size: 3.9 MB (3875757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3277f4f87432620a37e3aa7a47954d3cf169efb2131a0d9fe8dfedc6ce3d461b`  
		Last Modified: Thu, 21 Apr 2022 09:55:35 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbcb6c15b947cd08ea74086c0d6dc455f6ead2fca72a83a758b6f334ac4ec413`  
		Last Modified: Thu, 21 Apr 2022 09:55:36 GMT  
		Size: 1.3 MB (1336118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00177879e49a97a5b586558a0d87cf5440883302e19eb77df6459a90fd2e985`  
		Last Modified: Thu, 21 Apr 2022 09:55:38 GMT  
		Size: 6.2 MB (6185622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253fa72cc5d70cc9794fa2f8d288a2032b413110083f92161605f095310c6f1e`  
		Last Modified: Thu, 21 Apr 2022 09:55:34 GMT  
		Size: 1.1 MB (1097110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3662c97846d60d8e720bca2261af9de33a591425a77e04066500c29bf271aa47`  
		Last Modified: Thu, 21 Apr 2022 09:55:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f50c6456c2f66633a0f5f5b48def9ef146946eb2cb331352b1c1e081f45622`  
		Last Modified: Thu, 21 Apr 2022 09:55:34 GMT  
		Size: 5.6 KB (5585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f1718bb2885cc4b5b3838e3b6834d8ef4226be8ea82c9a0ae31e055c0c203`  
		Last Modified: Thu, 21 Apr 2022 09:57:30 GMT  
		Size: 35.8 MB (35798140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91017adb679749b7d1babf071f8225d2d758342002491485412d1a6502c7477`  
		Last Modified: Thu, 21 Apr 2022 09:57:04 GMT  
		Size: 8.1 KB (8082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a977dfe4c544c72a947eee4ef57018165d191ccabe64cac0a76097c5e406883`  
		Last Modified: Thu, 21 Apr 2022 09:57:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b52dc11bcb928182ff7a2c5b70c6b5f60bfee205b6084f4de3629da4a51d4`  
		Last Modified: Thu, 21 Apr 2022 09:57:04 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4481e34f9d780a216b80289c2f4718ec6f938ae6d8477159e1fe95e7a1c5c2e4`  
		Last Modified: Thu, 21 Apr 2022 09:57:04 GMT  
		Size: 4.7 KB (4708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce5fb32d42bba02f97c9ca7550eb1c96c08cf86b897927d72f2fdb5fc3ef507`  
		Last Modified: Thu, 21 Apr 2022 09:57:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:af51019e271f33b0d591ed99fa3101a2fa04e7490f8e403d6dc886d2ea3bb12f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (69980061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ace11f0a706fb8b2f5c2deac0cf004f2606f2b696b86f057ac7a070ad4265050`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 11 May 2022 00:49:23 GMT
ADD file:2da23cbf134c6ddbf47e6a21fd94f5d08453f8ea5b6d8c101c8a55408e61162c in / 
# Wed, 11 May 2022 00:49:24 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:56:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 07:56:44 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 11 May 2022 07:56:45 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 07:56:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 07:57:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 11 May 2022 07:57:05 GMT
ENV LANG=en_US.utf8
# Wed, 11 May 2022 07:57:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:57:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 07:57:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 08:07:30 GMT
ENV PG_MAJOR=10
# Wed, 11 May 2022 08:07:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 11 May 2022 08:07:32 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Wed, 11 May 2022 08:16:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 11 May 2022 08:16:15 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 11 May 2022 08:16:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 11 May 2022 08:16:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 11 May 2022 08:16:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 11 May 2022 08:16:19 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 11 May 2022 08:16:21 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 11 May 2022 08:16:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 May 2022 08:16:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 08:16:23 GMT
STOPSIGNAL SIGINT
# Wed, 11 May 2022 08:16:24 GMT
EXPOSE 5432
# Wed, 11 May 2022 08:16:25 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:716cebb420f77090ed0f738eb4ff36a4aff63f4b8bd8ad1e9fa099b3e2a53961`  
		Last Modified: Wed, 11 May 2022 00:57:53 GMT  
		Size: 20.4 MB (20423950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f28654705d5e9bce15eebb9b1530263b0cad0c143ac5ac706e1ff205acbedf`  
		Last Modified: Wed, 11 May 2022 08:20:13 GMT  
		Size: 3.9 MB (3890906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53421761fcfb66be9fe86bc42c40a7652676b525748f32d94b83e6c5ceb863c3`  
		Last Modified: Wed, 11 May 2022 08:20:12 GMT  
		Size: 1.7 KB (1661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c5b23e6ad13d97bc4767064725465579719ede8c74b8666b2cf0235c283261`  
		Last Modified: Wed, 11 May 2022 08:20:12 GMT  
		Size: 1.3 MB (1307854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc7b1cb6e6f71857a848267d9ebf482f5b6a30d8d33b5a7ec52d6d735516dd3`  
		Last Modified: Wed, 11 May 2022 08:20:11 GMT  
		Size: 6.2 MB (6182598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e6e2b71348b7e8a25f8da45752d6931e3db480388daad7a1f0c8a05e55275b`  
		Last Modified: Wed, 11 May 2022 08:20:10 GMT  
		Size: 1.0 MB (1007512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ecbb71ad65e93d931ef51fa7a75eda676d1252ed3abf4c57774c7de597e682`  
		Last Modified: Wed, 11 May 2022 08:20:10 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7465da7e2008b84ca962be1eb1071a8ef5a2f368c0992e1e68c92c96f8e67cee`  
		Last Modified: Wed, 11 May 2022 08:20:10 GMT  
		Size: 5.5 KB (5527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7519ad938eaf1311164bb5638d144a55f35d61f4e4067e6482df85892dd6f733`  
		Last Modified: Wed, 11 May 2022 08:21:02 GMT  
		Size: 37.1 MB (37146737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c891ac33780987453923cae3cd9f3d12f4c1395e74ef0311b1317d8f87e021`  
		Last Modified: Wed, 11 May 2022 08:20:54 GMT  
		Size: 8.1 KB (8072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63892736825514a0ba1e18f63066b358a859848f63317da832407dbff487961`  
		Last Modified: Wed, 11 May 2022 08:20:54 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8f01510dfc1f991da08a4948a295f5ea3d80267e87e75f2869470850ae44f5`  
		Last Modified: Wed, 11 May 2022 08:20:54 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c94ffbccaff306e2036a66661531803fa45fe59e34dc0cc54aa1f51fd07382`  
		Last Modified: Wed, 11 May 2022 08:20:54 GMT  
		Size: 4.7 KB (4708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b989d49c00da2faeef1c4a0b112cf28529c2188b16ec57a00244076eda9d3d`  
		Last Modified: Wed, 11 May 2022 08:20:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; 386

```console
$ docker pull postgres@sha256:d2eb15fa0faa01b6047c2f154db69e863d2f2d3854732baaa8a611074bb0c037
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74841711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:279ac4b506420d881100cbeb2d1a4a3eb96eb37f4ddd31bc96defe2320f2406c`
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
# Wed, 11 May 2022 10:35:37 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Wed, 11 May 2022 10:35:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 11 May 2022 10:35:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 11 May 2022 10:35:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 11 May 2022 10:35:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 11 May 2022 10:35:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 11 May 2022 10:35:59 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 11 May 2022 10:36:01 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 11 May 2022 10:36:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 11 May 2022 10:36:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 10:36:03 GMT
STOPSIGNAL SIGINT
# Wed, 11 May 2022 10:36:04 GMT
EXPOSE 5432
# Wed, 11 May 2022 10:36:05 GMT
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
	-	`sha256:65f7d2d884f5dfce59058cb084d5553a39c6958b70484ea393e7772666e3a2ab`  
		Last Modified: Wed, 11 May 2022 10:40:31 GMT  
		Size: 38.4 MB (38434573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c07541d702512e17323abd1d1cc834d9e9c3f986afea77cdd924f1fe0e46e`  
		Last Modified: Wed, 11 May 2022 10:40:24 GMT  
		Size: 8.1 KB (8070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7b0409bf01320a42044ce77936330672631bb6959404bc0e883af156d68fd2`  
		Last Modified: Wed, 11 May 2022 10:40:24 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c0f4494d062408b69451ec397fdb47a1cdf6809ced5f87637edb649cf35f80`  
		Last Modified: Wed, 11 May 2022 10:40:24 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cdb84d5ffcbc399ebd62ff6f6fdfbb8ff842b5f8348c4365db980fa1ca7d0d`  
		Last Modified: Wed, 11 May 2022 10:40:24 GMT  
		Size: 4.7 KB (4706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbac9c744a6d9ff715ed962667433698f0c3c2b4df7b32572878e4b5092e3976`  
		Last Modified: Wed, 11 May 2022 10:40:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
