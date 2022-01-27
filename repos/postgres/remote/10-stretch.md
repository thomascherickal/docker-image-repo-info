## `postgres:10-stretch`

```console
$ docker pull postgres@sha256:15d933c1a8f5d907280507da66bc741ffb30bd789f407ba04368c2f82b86c526
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
$ docker pull postgres@sha256:b77d94afc9aeabd1b0a3002b1736b3c9b32cc1657330b9e06fd06d2d0cd7d77b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73179179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03828c7b1e29e70b0b4aac2f1ea08c688564841775e6df3f7c30cd1171d99abc`
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
# Thu, 27 Jan 2022 01:13:59 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 27 Jan 2022 01:15:12 GMT
ENV PG_MAJOR=10
# Thu, 27 Jan 2022 01:15:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Thu, 27 Jan 2022 01:15:13 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Thu, 27 Jan 2022 01:15:28 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 27 Jan 2022 01:15:29 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 27 Jan 2022 01:15:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 27 Jan 2022 01:15:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 27 Jan 2022 01:15:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 27 Jan 2022 01:15:31 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 27 Jan 2022 01:15:32 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Thu, 27 Jan 2022 01:15:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 27 Jan 2022 01:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 01:15:33 GMT
STOPSIGNAL SIGINT
# Thu, 27 Jan 2022 01:15:33 GMT
EXPOSE 5432
# Thu, 27 Jan 2022 01:15:34 GMT
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
	-	`sha256:c63ad59a7dc5acc54bb98bd034207025fc4c7bbc68c0141dd94d21818ae5b6d7`  
		Last Modified: Thu, 27 Jan 2022 01:20:47 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e552f8007751831d77252c35685b2bf38e9074ea1d728ce72cf97361683c6c45`  
		Last Modified: Thu, 27 Jan 2022 01:22:05 GMT  
		Size: 38.2 MB (38175652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebc2d1bc399950bfc7df602386592c5ab230871e505534509c9b905564f68e6`  
		Last Modified: Thu, 27 Jan 2022 01:21:55 GMT  
		Size: 8.1 KB (8077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed0e00d10e2d4fa501ab46b38cf5560a347f1a2aae6b234d4c6cad729bd4930`  
		Last Modified: Thu, 27 Jan 2022 01:21:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e2065268c390a365031c99c5288097ad912be8adf2bb942878825b84254c46`  
		Last Modified: Thu, 27 Jan 2022 01:21:56 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c532a1b3820bdb75b942fa6907601d05dc1b16bfd722f75fc809e5cf1cb887`  
		Last Modified: Thu, 27 Jan 2022 01:21:56 GMT  
		Size: 4.7 KB (4723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f90792e4113c2970bf39e3a34464e2ffc192145ee63737bf3154e525e1f657`  
		Last Modified: Thu, 27 Jan 2022 01:21:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:ca151503394e3407757b5a4fd327f9aa7b8eb5ce557b6846539306887560d38b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70230792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa6df74447558a6248f94522b22ba96ade829175540968c33bea77defcc3fd87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 01:56:04 GMT
ADD file:aecbb416a4fc51bd94ece438e1bd6524edbf787b4c484441099d632362901e38 in / 
# Tue, 21 Dec 2021 01:56:05 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 09:57:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 09:57:13 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 09:57:13 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 09:57:48 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 09:58:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 09:58:08 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 09:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 09:58:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 09:58:29 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 10:48:51 GMT
ENV PG_MAJOR=10
# Tue, 21 Dec 2021 10:48:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 21 Dec 2021 10:48:52 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Tue, 21 Dec 2021 11:14:46 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 11:14:48 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 11:14:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 11:14:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 11:14:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 11:14:52 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:50:23 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:50:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 04 Jan 2022 01:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:50:26 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:50:26 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:50:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0f3f680c3c368352d3f8a6d5f8da1585e418328e6d555c1683259dec8380b822`  
		Last Modified: Tue, 21 Dec 2021 02:13:43 GMT  
		Size: 21.2 MB (21203490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6c2fe32a9a570d805d7a0093c5ea1dad7e909e1a4fc969dafa20e62e06810e`  
		Last Modified: Tue, 21 Dec 2021 12:11:39 GMT  
		Size: 4.2 MB (4239352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe957218a99b5e3d65eb5b0ae17bc2b7bc1efcb231fcf088bb09a2016239324`  
		Last Modified: Tue, 21 Dec 2021 12:11:38 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d487a5a1067d89c1a5fa656c7ca84c7c98d7d73721d74249fbc7c436a72223`  
		Last Modified: Tue, 21 Dec 2021 12:11:38 GMT  
		Size: 1.3 MB (1344241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899151a760bf8ed57c6e0426f55a2e63f0bef4edd45bf624fdbc9582b223693b`  
		Last Modified: Tue, 21 Dec 2021 12:11:39 GMT  
		Size: 6.2 MB (6185688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa4c7d49f3c691b9375a666d245b9697f1fc5352826c8c67fd7110ea41b3f97`  
		Last Modified: Tue, 21 Dec 2021 12:11:35 GMT  
		Size: 385.1 KB (385058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9efa7dd5d1e2ca9700ba358743a07f79de9f656930470e7527b0e2a3eb54536`  
		Last Modified: Tue, 21 Dec 2021 12:11:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a95f668b9ff79a36a8c9f8868de1ea2d06decd8a7a9edd763b38da68567548`  
		Last Modified: Tue, 21 Dec 2021 12:11:35 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdedfe3e02ef99f97b6812941a7d9948385f74c3eab5071fc427f4c48f192904`  
		Last Modified: Tue, 21 Dec 2021 12:13:22 GMT  
		Size: 36.9 MB (36852407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69737cec585e8ce940d685c0a7df66e5cca8e01c29ccf14b2d697c57b9750ed`  
		Last Modified: Tue, 21 Dec 2021 12:12:54 GMT  
		Size: 8.1 KB (8085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4d3bc372150937b8e5ea2976043812454bbfe4feeacf974352538fc4d64f12`  
		Last Modified: Tue, 21 Dec 2021 12:12:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bf6c6e6a80fe8130e1cf7bd51a1c8f06a4449767a5fa088d9a6b808ebb14ee`  
		Last Modified: Tue, 21 Dec 2021 12:12:54 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f36bf6b20b124166ef19f516d9290b70d1921f42eb68141a8a5dc9f10c39ea8`  
		Last Modified: Tue, 04 Jan 2022 01:55:41 GMT  
		Size: 4.7 KB (4725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ea83bbced7fbe750a799dce9d498cb14f63c59faa321886525f4cf1bfd62a2`  
		Last Modified: Tue, 04 Jan 2022 01:55:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:9556ec41d9e7a59c5eba20710e560968cf864cddc181971c1c24644bfa1a926f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66903201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbe505776cb7ef117a71f404c19c3a205ce25905ddf696b1dcf3b28cc2e14d0`
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
# Thu, 27 Jan 2022 04:25:03 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 27 Jan 2022 05:10:19 GMT
ENV PG_MAJOR=10
# Thu, 27 Jan 2022 05:10:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Thu, 27 Jan 2022 05:10:20 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Thu, 27 Jan 2022 05:33:25 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 27 Jan 2022 05:33:27 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 27 Jan 2022 05:33:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 27 Jan 2022 05:33:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 27 Jan 2022 05:33:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 27 Jan 2022 05:33:31 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 27 Jan 2022 05:33:32 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Thu, 27 Jan 2022 05:33:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 27 Jan 2022 05:33:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 05:33:34 GMT
STOPSIGNAL SIGINT
# Thu, 27 Jan 2022 05:33:35 GMT
EXPOSE 5432
# Thu, 27 Jan 2022 05:33:35 GMT
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
	-	`sha256:277344403a7c81936a1458ce96b9b9022ecbed1c599c987de057bc3610e97472`  
		Last Modified: Thu, 27 Jan 2022 06:27:54 GMT  
		Size: 5.3 KB (5349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20107fad6a51fcbdffc5064dc2da7c30b948b86615e0db08d733771ac594eb6c`  
		Last Modified: Thu, 27 Jan 2022 06:29:38 GMT  
		Size: 35.8 MB (35787498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dcea9f9b354ffd48f7c4c586542aeb26408e41b46525a2b15270b271e705ec`  
		Last Modified: Thu, 27 Jan 2022 06:29:12 GMT  
		Size: 8.1 KB (8081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9d3937d3ec60ea919de6a6ba3adddea837bf02edfb8ba6f8d01495f28ffd24`  
		Last Modified: Thu, 27 Jan 2022 06:29:12 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb3e28ecf7a15360297a691cfa5d6acefe02d415db1910fd4ed8188e64c8c21`  
		Last Modified: Thu, 27 Jan 2022 06:29:12 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157b2cdfb88e6f27932c7989606d9f937efe6cfc70a4d5cefc54c472da9bbe0a`  
		Last Modified: Thu, 27 Jan 2022 06:29:12 GMT  
		Size: 4.7 KB (4728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb384872312354ef328beba611c914960f2bb98539d71e728d3d2440a5572a84`  
		Last Modified: Thu, 27 Jan 2022 06:29:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:fa234f8837292df754efdae5c65c7408e63ec5a8074e7d190030b0404a1f3d5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69110835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c834538c7c35e44dbb0f575ddc55d3b005651ddc4fd58a98f71f26c3e5c06e56`
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
# Wed, 26 Jan 2022 06:37:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 26 Jan 2022 06:47:09 GMT
ENV PG_MAJOR=10
# Wed, 26 Jan 2022 06:47:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 26 Jan 2022 06:47:11 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Wed, 26 Jan 2022 06:55:44 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 26 Jan 2022 06:55:45 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 26 Jan 2022 06:55:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 26 Jan 2022 06:55:47 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 26 Jan 2022 06:55:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 26 Jan 2022 06:55:49 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 26 Jan 2022 06:55:51 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Wed, 26 Jan 2022 06:55:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 26 Jan 2022 06:55:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 06:55:53 GMT
STOPSIGNAL SIGINT
# Wed, 26 Jan 2022 06:55:54 GMT
EXPOSE 5432
# Wed, 26 Jan 2022 06:55:55 GMT
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
	-	`sha256:6bbb04bdc22bd0ca9ad7096ac2bca260df79bd49c36554a2c4c8c6d11310a2f4`  
		Last Modified: Wed, 26 Jan 2022 07:10:01 GMT  
		Size: 5.3 KB (5318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb917bcb8cfd03f73d3e3dc1a81386dc8e7d7606b170a7e3b1128dba76d4de`  
		Last Modified: Wed, 26 Jan 2022 07:11:01 GMT  
		Size: 37.1 MB (37147017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236c32dd0679ab15a74f680c6eb50e21e8b1c698292c44dadae459e3c25f6e59`  
		Last Modified: Wed, 26 Jan 2022 07:10:51 GMT  
		Size: 8.1 KB (8073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bf06cf08fe51bb3adc267131ce85ebcdc1b875dd1303ae1f05fa32f97d7365`  
		Last Modified: Wed, 26 Jan 2022 07:10:51 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a6a83743de50d62ecfc7ee1822ca1c8747c7f8aab12640d7503ce3682f0856`  
		Last Modified: Wed, 26 Jan 2022 07:10:51 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4e37434643dc83272b2b2bbece69d20cb89f2d20c407509619e886a4ccf3d8`  
		Last Modified: Wed, 26 Jan 2022 07:10:51 GMT  
		Size: 4.7 KB (4729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d405f4ad33ac8396411cfb1702e6645094064a70cbaf18680a0cd0e26645682c`  
		Last Modified: Wed, 26 Jan 2022 07:10:51 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; 386

```console
$ docker pull postgres@sha256:bba7ed1428c48ce3f6ba43a6e78c1aa23e0841c1beae871224f1d17f10a1874b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74340695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f00cb82eeb00f30999904a2e7a222b34927a0a9d6bf9d5e15cfb820d24b77d`
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
# Wed, 26 Jan 2022 20:40:36 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 26 Jan 2022 20:52:49 GMT
ENV PG_MAJOR=10
# Wed, 26 Jan 2022 20:52:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 26 Jan 2022 20:52:49 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Wed, 26 Jan 2022 20:53:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 26 Jan 2022 20:53:08 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 26 Jan 2022 20:53:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 26 Jan 2022 20:53:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 26 Jan 2022 20:53:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 26 Jan 2022 20:53:10 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 26 Jan 2022 20:53:11 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Wed, 26 Jan 2022 20:53:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 26 Jan 2022 20:53:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 20:53:12 GMT
STOPSIGNAL SIGINT
# Wed, 26 Jan 2022 20:53:12 GMT
EXPOSE 5432
# Wed, 26 Jan 2022 20:53:13 GMT
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
	-	`sha256:7c6176a31fc2b0806a0560d5f59386f4f519de6741a7404319fe5808a07f2fea`  
		Last Modified: Wed, 26 Jan 2022 21:11:04 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de3540951070296169da85501354265a35d4dec3850058353940d389518c25d`  
		Last Modified: Wed, 26 Jan 2022 21:12:19 GMT  
		Size: 38.4 MB (38424486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574364a673384c7f7c69be0083f3daa46c1d5f3a4b812ce4edb917840e1960a3`  
		Last Modified: Wed, 26 Jan 2022 21:12:07 GMT  
		Size: 8.1 KB (8080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d390388a8298ee9570c2ae70b3baf6cdeba1bddda229eb79320c0bcbcb55348a`  
		Last Modified: Wed, 26 Jan 2022 21:12:08 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af573deb3cc94c8bd063de75d971485134abab6154397a9904553e529f21a398`  
		Last Modified: Wed, 26 Jan 2022 21:12:07 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9bf378228dc8fbf11287860c0532d017714d370ad39c4496fdbdfd3b1b6711`  
		Last Modified: Wed, 26 Jan 2022 21:12:07 GMT  
		Size: 4.7 KB (4723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71aac38031856c9d93a8b79057ccd023ad7af9a22fe4b766a733fa07e1ac4887`  
		Last Modified: Wed, 26 Jan 2022 21:12:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
