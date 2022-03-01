## `postgres:11-stretch`

```console
$ docker pull postgres@sha256:e17d8839fd17f0a7cdc8faad4a3012f0787d643e3eb37198b0e9e82594fb4012
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
$ docker pull postgres@sha256:06abf89bb0f531598fcdce393da360a2061c994932f52684c10d4a4c3d6aa94a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106547880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec851dfc6996161f9ec1941d2ae909a8bebf10039817c6043709c093a33fca3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:57 GMT
ADD file:bed2454356c48f77207726865f8aee34a5b3db6927a881655573cbde13ce5a89 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 01:12:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 01:12:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 27 Jan 2022 01:12:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 01:13:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 01:13:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 27 Jan 2022 01:13:07 GMT
ENV LANG=en_US.utf8
# Thu, 27 Jan 2022 01:13:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 01:13:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 12 Feb 2022 00:51:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 12 Feb 2022 00:51:41 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 00:51:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sat, 12 Feb 2022 00:51:42 GMT
ENV PG_VERSION=11.15-1.pgdg90+1
# Mon, 14 Feb 2022 22:10:33 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			apt-get install -y --no-install-recommends clang-6.0; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Mon, 14 Feb 2022 22:10:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Mon, 14 Feb 2022 22:10:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 14 Feb 2022 22:10:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 14 Feb 2022 22:10:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 14 Feb 2022 22:10:36 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 14 Feb 2022 22:10:36 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Mon, 14 Feb 2022 22:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Feb 2022 22:10:37 GMT
STOPSIGNAL SIGINT
# Mon, 14 Feb 2022 22:10:37 GMT
EXPOSE 5432
# Mon, 14 Feb 2022 22:10:37 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1cb79db8a9e79b4f5415eaa91602251fb1eafe68d236efb80fe931bacfe5b3d6`  
		Last Modified: Wed, 26 Jan 2022 01:51:06 GMT  
		Size: 22.5 MB (22529131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bae7873dd71bd3cea341cc690441e65addb698e9fa441e5916688f7b351702`  
		Last Modified: Thu, 27 Jan 2022 01:20:52 GMT  
		Size: 4.5 MB (4503856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7722dc50a79f5c491ef429c4e1cedf06cd92d57fd81d4128606dd4d19e3193`  
		Last Modified: Thu, 27 Jan 2022 01:20:49 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8622b8cb6f3d0dbfe4c1ab447f2d1f8be3551910639df6dee3e3947851a109c`  
		Last Modified: Thu, 27 Jan 2022 01:20:50 GMT  
		Size: 1.4 MB (1379391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d74bba3a57b1c5b053a685119ac3f792efd9b170a2ccdb896f7f9ff30593a8`  
		Last Modified: Thu, 27 Jan 2022 01:20:49 GMT  
		Size: 6.2 MB (6185587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874d4d2a09fd5b796094b58b54495e8ccf587b2206cfecd9c1ba981700c156ba`  
		Last Modified: Thu, 27 Jan 2022 01:20:48 GMT  
		Size: 385.0 KB (385015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d87c3a4038c4fe58c5c23882d960a2cad96560f9d3038c97f644174c3a0172e`  
		Last Modified: Thu, 27 Jan 2022 01:20:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f955a6cf127bd643a6401f99e2a4a9928f96b956fba4e6c810ddea164d30efbd`  
		Last Modified: Sat, 12 Feb 2022 01:09:05 GMT  
		Size: 5.6 KB (5588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c607e7071388dc8db9a0abba258e30650b6740f3e47054259d90d7ca2de432e7`  
		Last Modified: Mon, 14 Feb 2022 22:15:17 GMT  
		Size: 71.5 MB (71544007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1026a7bbc62f28d3ba59c7be773cc68a5d69fa77266dad529896e93af9db0e29`  
		Last Modified: Mon, 14 Feb 2022 22:15:07 GMT  
		Size: 8.3 KB (8329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1ba5d59f0eff6ec6fc8422bfbc9a997f3cd41849545df435843c9e5346ba5a`  
		Last Modified: Mon, 14 Feb 2022 22:15:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915b4028528fb3f3750409d59a9dd26602d3287fc8f8aaabac3018afe58caebf`  
		Last Modified: Mon, 14 Feb 2022 22:15:07 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd826953df80a75914b6a11c53fb1f653be090dc6c55c1dfd0a5859b37430ac`  
		Last Modified: Mon, 14 Feb 2022 22:15:07 GMT  
		Size: 4.7 KB (4691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:174705a55fa56acf714e630403dbcb575f663f8622ec0f230dcacf6a927417cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70719197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc91815d074d555ee8f4df3b5f3c7cf8bc7b5fd0c64c119956d8fa8f204280ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:47 GMT
ADD file:7ba67de2da2d36a62cc2408396fc8c8571ddec0f9e54398459b261e0ce1f73f2 in / 
# Tue, 01 Mar 2022 02:08:48 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 11:49:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 11:49:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 01 Mar 2022 11:49:22 GMT
ENV GOSU_VERSION=1.14
# Tue, 01 Mar 2022 11:49:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 01 Mar 2022 11:50:13 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 01 Mar 2022 11:50:13 GMT
ENV LANG=en_US.utf8
# Tue, 01 Mar 2022 11:50:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 11:50:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 01 Mar 2022 11:50:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 01 Mar 2022 11:50:42 GMT
ENV PG_MAJOR=11
# Tue, 01 Mar 2022 11:50:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 01 Mar 2022 11:50:43 GMT
ENV PG_VERSION=11.15-1.pgdg90+1
# Tue, 01 Mar 2022 12:17:27 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			apt-get install -y --no-install-recommends clang-6.0; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 01 Mar 2022 12:17:29 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 01 Mar 2022 12:17:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 01 Mar 2022 12:17:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 01 Mar 2022 12:17:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 01 Mar 2022 12:17:33 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 01 Mar 2022 12:17:34 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Tue, 01 Mar 2022 12:17:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 12:17:35 GMT
STOPSIGNAL SIGINT
# Tue, 01 Mar 2022 12:17:35 GMT
EXPOSE 5432
# Tue, 01 Mar 2022 12:17:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e1fc40b579c554284072c098e17ce2034889200a36f1168e6e6baed4aab3de88`  
		Last Modified: Tue, 01 Mar 2022 02:26:15 GMT  
		Size: 21.2 MB (21203497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c689fb7ed4fdeb91555c0b99fc82eff808b671328b2d7c193c9acbd86cd6bd`  
		Last Modified: Tue, 01 Mar 2022 13:14:42 GMT  
		Size: 4.2 MB (4239326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d64d4f1e21cceae6a9fc597346f378615938e862918cccde533bfd2e6ea80b1`  
		Last Modified: Tue, 01 Mar 2022 13:14:39 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e9e26bdff95dce3f564a6205ba99fb9badd4998a74d58ae90ad2d0538be1ee`  
		Last Modified: Tue, 01 Mar 2022 13:14:39 GMT  
		Size: 1.3 MB (1344213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17883ce8a8be20fbf3d79222d5204641c7c3af1f5c566a6ecd2c4659e44fbc9f`  
		Last Modified: Tue, 01 Mar 2022 13:14:42 GMT  
		Size: 6.2 MB (6185706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b34dd189586a8519479d842cc5f10718624c106ebd9a8e029a8083f7f10de0`  
		Last Modified: Tue, 01 Mar 2022 13:14:38 GMT  
		Size: 385.0 KB (385040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1eee84502d565effc8bfb84dc369cd72b6aa0ce4a3b6d05a3d00edbab933af`  
		Last Modified: Tue, 01 Mar 2022 13:14:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713463f797a80095c136cab9f4744032898890aee3897bb132d72bbe4fa18738`  
		Last Modified: Tue, 01 Mar 2022 13:14:37 GMT  
		Size: 5.6 KB (5583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7246eeb5a2f4593eab498ed369c2c9e44de7377e9f9057683b01329ed748f23f`  
		Last Modified: Tue, 01 Mar 2022 13:15:02 GMT  
		Size: 37.3 MB (37340531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1441efc8ed56d812f31074f51b61df40fe9684e590b24aa82a45e2d6507ca89d`  
		Last Modified: Tue, 01 Mar 2022 13:14:36 GMT  
		Size: 8.3 KB (8330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b834bc7cd7ea68124084ce4ea4b5f7aa9b6c7e57a6e461c5509c387e7f4e9e`  
		Last Modified: Tue, 01 Mar 2022 13:14:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3cd630b01bee2d6ab00951dde3d99d6b366447d424842532e26ccd029399dd`  
		Last Modified: Tue, 01 Mar 2022 13:14:36 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bbbf4d6d9f16916ea64060bab078751fc835206b65ffaa911fd05cdce8ce8e`  
		Last Modified: Tue, 01 Mar 2022 13:14:36 GMT  
		Size: 4.7 KB (4689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:9204db4feda2545709e6425f8d768677cce7a382cbf93ab16629ccd8f1b2794b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67359307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df74f14413c850b1903da1df6f0420ce5b43ab87538c905781c6674d6dca2fc1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:08 GMT
ADD file:26e6c9015d58ffb5e67d6ea64451fd0e27a9a60c65340659b35b075d51ed5c45 in / 
# Wed, 26 Jan 2022 01:48:09 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 04:23:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 Jan 2022 04:23:33 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 27 Jan 2022 04:23:34 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 04:24:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 04:24:31 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 27 Jan 2022 04:24:32 GMT
ENV LANG=en_US.utf8
# Thu, 27 Jan 2022 04:24:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 04:24:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 12 Feb 2022 01:35:31 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 12 Feb 2022 01:35:32 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 01:35:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sat, 12 Feb 2022 01:35:33 GMT
ENV PG_VERSION=11.15-1.pgdg90+1
# Tue, 15 Feb 2022 01:23:26 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			apt-get install -y --no-install-recommends clang-6.0; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 15 Feb 2022 01:23:28 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 15 Feb 2022 01:23:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 15 Feb 2022 01:23:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 15 Feb 2022 01:23:32 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 15 Feb 2022 01:23:33 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 15 Feb 2022 01:23:33 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Tue, 15 Feb 2022 01:23:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Feb 2022 01:23:34 GMT
STOPSIGNAL SIGINT
# Tue, 15 Feb 2022 01:23:35 GMT
EXPOSE 5432
# Tue, 15 Feb 2022 01:23:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b651abcd2676c0bd22abf9acddc50231c15d43b1004fd0446bb57150c0d4c96b`  
		Last Modified: Wed, 26 Jan 2022 02:05:54 GMT  
		Size: 19.3 MB (19318809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896eb92fb6a13b39352f83a11a440d9eb0ae302d0fec21eb45f18fa2a847d4a2`  
		Last Modified: Thu, 27 Jan 2022 06:27:58 GMT  
		Size: 3.9 MB (3875586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9507907b3074ab6dbd2b3736c143ea3ce4f4f544e0aae266e3c41daf1fa9f6`  
		Last Modified: Thu, 27 Jan 2022 06:27:56 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53a690926100efda80bec721eb1313e3e6f3dd8668533dba3b00d4082d6592d`  
		Last Modified: Thu, 27 Jan 2022 06:27:56 GMT  
		Size: 1.3 MB (1335869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa4762b46a9eee5e37436b04babcddbbfe621d857e8c1eb54380e947873fb29`  
		Last Modified: Thu, 27 Jan 2022 06:27:58 GMT  
		Size: 6.2 MB (6185715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583591e6d5fa9fd381e4d2c0f043a15d6e21c2df302d366131d536e785ae50ee`  
		Last Modified: Thu, 27 Jan 2022 06:27:54 GMT  
		Size: 379.2 KB (379167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc905e6a4dd33d111191ade266dddaa8f132d3e1334e7f62652f57eca43f2a6`  
		Last Modified: Thu, 27 Jan 2022 06:27:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbe604e653b730767f4104f7807163146c05b937663b66faba8ac9caa3fb92`  
		Last Modified: Sat, 12 Feb 2022 03:24:43 GMT  
		Size: 5.6 KB (5588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca18ea15a3935ce786efe27d7fb64ae4f3dc543891d710eec45e1cc99184f50`  
		Last Modified: Tue, 15 Feb 2022 02:19:46 GMT  
		Size: 36.2 MB (36243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55940088b473c03961475b9e3a0e1fdf41c6220d6895cecac6948320ac394ad7`  
		Last Modified: Tue, 15 Feb 2022 02:19:22 GMT  
		Size: 8.3 KB (8332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae992dd30a339b039b345d5cc3c97609e0bb353c884837fc217745ee4f778f0c`  
		Last Modified: Tue, 15 Feb 2022 02:19:22 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cb66b1173b3731eb9dd1118c6c3ea91b593402f4916c895e7707b3b7294014`  
		Last Modified: Tue, 15 Feb 2022 02:19:22 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffa25b58318a18bbf7640f30d5b7c291a1e3eab927e0fa5c2cea45513e5443`  
		Last Modified: Tue, 15 Feb 2022 02:19:22 GMT  
		Size: 4.7 KB (4694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:f350bae692217b59dfecf0f853fcaa852cbdd44374a56a1e11ff85530d1c48da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69581418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf9b1a5a78e54acf7db4382ee16e371589bf8e41a749f76c8be112705031056`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:48 GMT
ADD file:952345b92a37bdbcaea817a1a9e1466c68e040b5dee856ff2606afbd1297b1f0 in / 
# Wed, 26 Jan 2022 01:44:48 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 06:36:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 06:36:33 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 26 Jan 2022 06:36:34 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Jan 2022 06:36:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Jan 2022 06:36:52 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 26 Jan 2022 06:36:53 GMT
ENV LANG=en_US.utf8
# Wed, 26 Jan 2022 06:36:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:36:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 12 Feb 2022 01:02:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 12 Feb 2022 01:02:21 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 01:02:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sat, 12 Feb 2022 01:02:23 GMT
ENV PG_VERSION=11.15-1.pgdg90+1
# Tue, 15 Feb 2022 00:31:32 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			apt-get install -y --no-install-recommends clang-6.0; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 15 Feb 2022 00:31:33 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 15 Feb 2022 00:31:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 15 Feb 2022 00:31:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 15 Feb 2022 00:31:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 15 Feb 2022 00:31:37 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 15 Feb 2022 00:31:39 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Tue, 15 Feb 2022 00:31:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Feb 2022 00:31:40 GMT
STOPSIGNAL SIGINT
# Tue, 15 Feb 2022 00:31:41 GMT
EXPOSE 5432
# Tue, 15 Feb 2022 00:31:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0baeb81232d08980c2f78646547d7792710a684e89313d2da7499bdff69437d0`  
		Last Modified: Wed, 26 Jan 2022 01:53:21 GMT  
		Size: 20.4 MB (20389407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0d2feedd824ec314ddc4ba8a4b653f218fc8f3a6bfcfe9846a81d11cf392ce`  
		Last Modified: Wed, 26 Jan 2022 07:10:06 GMT  
		Size: 3.9 MB (3890633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04fdad564a5b91a6bb794e63c03507723b191ada9ad1b4af35edf61280b8f02`  
		Last Modified: Wed, 26 Jan 2022 07:10:04 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5ce0e066d50924f8cb1f56120cbe77fb4423d0d7ce1eeec7491afe306403a3`  
		Last Modified: Wed, 26 Jan 2022 07:10:04 GMT  
		Size: 1.3 MB (1307653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d75bd410a956ae87d5b030670fbe8105aad59885040705248537fc28d4b8c6`  
		Last Modified: Wed, 26 Jan 2022 07:10:04 GMT  
		Size: 6.2 MB (6182391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ec45cd92a9bd6fb3bdbe1c5a6179edef6618dac02b5dd90d44e35383f586a9`  
		Last Modified: Wed, 26 Jan 2022 07:10:01 GMT  
		Size: 173.4 KB (173415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5092dfc5d22cf071efa066421f0ec49adab687a4a761b0715ccffb85b50a65`  
		Last Modified: Wed, 26 Jan 2022 07:10:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c27d05cfd795456c60a6ba7315fa6c745fc0b50527bef6913d22de0a168e6`  
		Last Modified: Sat, 12 Feb 2022 01:42:47 GMT  
		Size: 5.5 KB (5529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e86313efdaf14ff63a577988c2890762aeae416e75c15ae86a2f6e575a3078`  
		Last Modified: Tue, 15 Feb 2022 00:46:00 GMT  
		Size: 37.6 MB (37617287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9967287946b438f37f12a4623870444cbd2313a372e38a68e51264a39a81c664`  
		Last Modified: Tue, 15 Feb 2022 00:45:53 GMT  
		Size: 8.3 KB (8332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6ca4da2bc92f4e90140442077d8e1949e8ea3f9cfe99d31ca724284f261db`  
		Last Modified: Tue, 15 Feb 2022 00:45:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84663f3c4a5ce199b47714eb888386828f0454ea244e2127d778d0511b3725`  
		Last Modified: Tue, 15 Feb 2022 00:45:53 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346cf25d3b9e39d70b167cadcb2afb8c578fdc585ab9d48c18d5612233dba103`  
		Last Modified: Tue, 15 Feb 2022 00:45:53 GMT  
		Size: 4.7 KB (4690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; 386

```console
$ docker pull postgres@sha256:3913db63cf6c4f04165d3677a80e4a0eeca2b61d77fcc9c2978c0cd6eee178f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (109987894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadd245dff118a07402e2b534dc0e80380abd9d0f36e8283ed62aebc34676b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:09 GMT
ADD file:1c29df24192bec213388520a67c5240faae6bd745b2564e5efdd60971bb2c790 in / 
# Wed, 26 Jan 2022 01:43:10 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 20:39:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 20:39:19 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 26 Jan 2022 20:39:19 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Jan 2022 20:39:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Jan 2022 20:39:45 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 26 Jan 2022 20:39:45 GMT
ENV LANG=en_US.utf8
# Wed, 26 Jan 2022 20:39:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:39:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 12 Feb 2022 00:26:00 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 12 Feb 2022 00:26:00 GMT
ENV PG_MAJOR=11
# Sat, 12 Feb 2022 00:26:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sat, 12 Feb 2022 00:26:01 GMT
ENV PG_VERSION=11.15-1.pgdg90+1
# Mon, 14 Feb 2022 23:27:51 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			apt-get install -y --no-install-recommends clang-6.0; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Mon, 14 Feb 2022 23:27:52 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Mon, 14 Feb 2022 23:27:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 14 Feb 2022 23:27:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 14 Feb 2022 23:27:55 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 14 Feb 2022 23:27:55 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 14 Feb 2022 23:27:56 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Mon, 14 Feb 2022 23:27:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Feb 2022 23:27:56 GMT
STOPSIGNAL SIGINT
# Mon, 14 Feb 2022 23:27:56 GMT
EXPOSE 5432
# Mon, 14 Feb 2022 23:27:56 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2c3e625e0e633ceda6a42ce6fe1ae47e63ec926578565fe21b3639252c2d230b`  
		Last Modified: Wed, 26 Jan 2022 01:54:28 GMT  
		Size: 23.2 MB (23157511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e2be1fd7f4df38e50faa2710905db9c34eff3016d8414355e129881b20d263`  
		Last Modified: Wed, 26 Jan 2022 21:11:09 GMT  
		Size: 4.8 MB (4811979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122510e1138c0c04f828489ab436784acbe1a982988b07027cab26e872d1b95f`  
		Last Modified: Wed, 26 Jan 2022 21:11:06 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc22bc6d63261ea1b5ab663beae2916e7b46c199bcf1e76bf0309a55b8a0668`  
		Last Modified: Wed, 26 Jan 2022 21:11:07 GMT  
		Size: 1.3 MB (1347234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b648c3229f91918a8c8778e9a5efd3939e73ce89c45691c14480987995cb7f45`  
		Last Modified: Wed, 26 Jan 2022 21:11:06 GMT  
		Size: 6.2 MB (6185628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d1e5b6e6a008241d8158286d5bf4639c56e424fa22e929480fcacb1424e68f`  
		Last Modified: Wed, 26 Jan 2022 21:11:04 GMT  
		Size: 393.3 KB (393306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069ec53d3a42a4d0d9953b81c4d2ff41363e38a5e993513ea8a057c208f7f64c`  
		Last Modified: Wed, 26 Jan 2022 21:11:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742c99e4085e9ab27580ec54a8d43a9063b368e57b3c6c1ba297ee41c24572ee`  
		Last Modified: Sat, 12 Feb 2022 01:11:40 GMT  
		Size: 5.6 KB (5560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8fb71100a48012706477e9dd2f97910eade4bbaa1502974406543bfa13169a`  
		Last Modified: Mon, 14 Feb 2022 23:42:50 GMT  
		Size: 74.1 MB (74071380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8086c5c2640a8802ae8fe2dbd7932a54c3a5fa3ba1f1dafedd7e2d4b5797d1`  
		Last Modified: Mon, 14 Feb 2022 23:42:37 GMT  
		Size: 8.3 KB (8325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8eb6d91a9b6d91b5fc6aa69fda299a9680a226665db883f969b39eb44b49b4`  
		Last Modified: Mon, 14 Feb 2022 23:42:37 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be18fca677a64a536462adea0168b5623b1fe90bc6f7f6a06666608ff1acae64`  
		Last Modified: Mon, 14 Feb 2022 23:42:37 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5db29d2d4d8ba30c1e10903d87b4872d7df628ec83351588c050ebde6dcc147`  
		Last Modified: Mon, 14 Feb 2022 23:42:37 GMT  
		Size: 4.7 KB (4688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
