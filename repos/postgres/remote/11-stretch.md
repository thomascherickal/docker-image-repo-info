## `postgres:11-stretch`

```console
$ docker pull postgres@sha256:96d5b7451e9171197059b3eebf635eb99684a7084c795f2fb3b43925b74ecf11
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
$ docker pull postgres@sha256:afbcae3e487f4ca8331fbb4c67e4eb7fab858c137ca6a75953dfc749d568c109
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106522024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dcb100ad2e762e32dbf9ccbaa76f4b0745fd12570eb35a7f9551fabd21fe9a7`
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
# Thu, 27 Jan 2022 01:13:59 GMT
ENV PG_MAJOR=11
# Thu, 27 Jan 2022 01:13:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 27 Jan 2022 01:14:00 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Thu, 27 Jan 2022 01:14:24 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 27 Jan 2022 01:14:26 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 27 Jan 2022 01:14:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 27 Jan 2022 01:14:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 27 Jan 2022 01:14:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 27 Jan 2022 01:14:28 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 27 Jan 2022 01:14:28 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Thu, 27 Jan 2022 01:14:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 01:14:29 GMT
STOPSIGNAL SIGINT
# Thu, 27 Jan 2022 01:14:29 GMT
EXPOSE 5432
# Thu, 27 Jan 2022 01:14:29 GMT
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
	-	`sha256:ec3399d17401676d6a20828000308b0bcfda9c69227e5a940370b37f669cd6b6`  
		Last Modified: Thu, 27 Jan 2022 01:20:59 GMT  
		Size: 71.5 MB (71518357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ae1b5a47f74bb61cf4e56840ee49452bc3e082f9b294a5985b725b91d15ba4`  
		Last Modified: Thu, 27 Jan 2022 01:20:44 GMT  
		Size: 8.3 KB (8331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251683572b67228cf23cc269069d628a5906867e5ce9478a0d256570bb554298`  
		Last Modified: Thu, 27 Jan 2022 01:20:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b2946395766abf06d93e3b3e642365d2fa9583c98c86ad80871bb732be9e21`  
		Last Modified: Thu, 27 Jan 2022 01:20:44 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cfd39a4400237619c6622f665b7b56ad9066d89925bba522c690c15c3ea18f`  
		Last Modified: Thu, 27 Jan 2022 01:20:43 GMT  
		Size: 4.7 KB (4727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:5efcfddb7591be8d9931b863bd224690df7a790e652526ee21c2c3a19f83d9bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70700661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:247da124c57fff1fa738dc8cf854ea5aa15c89cd010301df775e5e6942111637`
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
# Tue, 21 Dec 2021 09:58:29 GMT
ENV PG_MAJOR=11
# Tue, 21 Dec 2021 09:58:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 21 Dec 2021 09:58:30 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Tue, 21 Dec 2021 10:25:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 10:25:05 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 10:25:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 10:25:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 10:25:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 10:25:09 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:49:52 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:49:53 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:49:54 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:49:54 GMT
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
	-	`sha256:99526eae5626858bcd2f192964063450005e07a799adca1daef7d8e7339471e7`  
		Last Modified: Tue, 21 Dec 2021 12:12:00 GMT  
		Size: 37.3 MB (37322150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f792a61bd08a7ec0e9d1c90eb74bf7697180047310f02d91cd16a9155f6718`  
		Last Modified: Tue, 21 Dec 2021 12:11:33 GMT  
		Size: 8.3 KB (8330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a15768936dab5d99e8583bee5f12031d758725bbab53fb712215f30c696103b`  
		Last Modified: Tue, 21 Dec 2021 12:11:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cd3ab25e8061b1d05d9fa819503890f3c78e3995fbdfd1b1dfdc9cac8c9cc9`  
		Last Modified: Tue, 21 Dec 2021 12:11:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5696ee7dc125d8b0b43e723c5ff5bca1dec6c16e420eeca37ee522fc0e41a83`  
		Last Modified: Tue, 04 Jan 2022 01:55:07 GMT  
		Size: 4.7 KB (4726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:0a2d34f4559b3c1e915fa4dd3b1dd6a043843c230b899e4a98a5bc2a1d06d1b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67346633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3318adc789737266a0f459300c93628e05cb20c632f8ff193ee3c3f7cf6ab99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 02:05:40 GMT
ADD file:924a2e95e52f87fd6e79e8b0865e63f19432a71f823114b8b4d729ecd420d7fb in / 
# Tue, 21 Dec 2021 02:05:41 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 15:48:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 15:48:50 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 15:48:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 15:49:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 15:49:36 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 15:49:37 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 15:49:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 15:49:48 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 15:49:55 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 15:49:56 GMT
ENV PG_MAJOR=11
# Tue, 21 Dec 2021 15:49:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 21 Dec 2021 15:49:57 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Tue, 21 Dec 2021 16:13:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 16:13:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 16:13:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 16:13:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 16:13:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 16:13:14 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 00:59:56 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 00:59:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 00:59:57 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 00:59:58 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 00:59:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:12790d92cf90440e36a3292fe34a336c54030e049074eb36386502daa81decea`  
		Last Modified: Tue, 21 Dec 2021 02:22:43 GMT  
		Size: 19.3 MB (19318715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547c203a914faa94a6bdf997b47df45476466e3c6cfb5afb10354451667941f2`  
		Last Modified: Tue, 21 Dec 2021 17:53:07 GMT  
		Size: 3.9 MB (3875517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b600899c104248e32b211e0b101e36c8a34a1c8b06a59e2b4e3340de4dbca1e7`  
		Last Modified: Tue, 21 Dec 2021 17:53:05 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df7cd75b521287067788d1f241419bb2d2c56b67d943f0de1df7bb13df23cb`  
		Last Modified: Tue, 21 Dec 2021 17:53:05 GMT  
		Size: 1.3 MB (1335861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5a9e68d293957449e099c3091122902c3baf205a763d65bea162d702a78334`  
		Last Modified: Tue, 21 Dec 2021 17:53:07 GMT  
		Size: 6.2 MB (6185636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9f26646b0374d447c29161f8a7ee0fa1b6f7036d7cfdc82aa72e987b0a1967`  
		Last Modified: Tue, 21 Dec 2021 17:53:03 GMT  
		Size: 379.1 KB (379143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b88ad31962e800f7abf388a9cfcd68887f4341985ab4ee838be6cafb815261`  
		Last Modified: Tue, 21 Dec 2021 17:53:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9fa042d17dcc475d0f8b5013ecd97324f54009c2af40ec144db55113b63ae3`  
		Last Modified: Tue, 21 Dec 2021 17:53:03 GMT  
		Size: 4.8 KB (4793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76be3b78d5855f61170554da9c8d7915320c34561df5e894793d9a710632340e`  
		Last Modified: Tue, 21 Dec 2021 17:53:26 GMT  
		Size: 36.2 MB (36231620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6826d05fcfae3f7b0107b0628f30fcb5076990715ace2035b0fd4eedaa24f725`  
		Last Modified: Tue, 21 Dec 2021 17:53:01 GMT  
		Size: 8.3 KB (8334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc50b8046bf925002ef42414ade1c3f8e01c1ce1975e6e89f2a70c355b0f6f2`  
		Last Modified: Tue, 21 Dec 2021 17:53:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5648b5c88bf098bcea290c3b76275afb5236f33ffae1a391cf97b9e6926b153`  
		Last Modified: Tue, 21 Dec 2021 17:53:01 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8367c5fcbfd9fe5435af47e66dc984eae7344473cf7f4e36e08591fc95c1a5aa`  
		Last Modified: Tue, 04 Jan 2022 01:09:27 GMT  
		Size: 4.7 KB (4727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:3844c20e1325fa41086c87b1de8d617800d698f43fa1a6da61931e79bc33e948
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69573362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da558b81361e000ccf0439a3ada82569215c4cab1f3970de43b7ba52ddc9e0`
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
# Wed, 26 Jan 2022 06:37:10 GMT
ENV PG_MAJOR=11
# Wed, 26 Jan 2022 06:37:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Wed, 26 Jan 2022 06:37:12 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Wed, 26 Jan 2022 06:46:00 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 26 Jan 2022 06:46:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 26 Jan 2022 06:46:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 26 Jan 2022 06:46:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 26 Jan 2022 06:46:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 26 Jan 2022 06:46:04 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 26 Jan 2022 06:46:06 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Wed, 26 Jan 2022 06:46:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 06:46:07 GMT
STOPSIGNAL SIGINT
# Wed, 26 Jan 2022 06:46:08 GMT
EXPOSE 5432
# Wed, 26 Jan 2022 06:46:09 GMT
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
	-	`sha256:fe324828d476becc110caf7a0473a0be7858e6f611f745595e5c0f88c85c4c1f`  
		Last Modified: Wed, 26 Jan 2022 07:10:06 GMT  
		Size: 37.6 MB (37609410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3267be30bf7a0ae357858c534862d171ef4f6b4eda6a407636654e783053370`  
		Last Modified: Wed, 26 Jan 2022 07:09:59 GMT  
		Size: 8.3 KB (8328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813829bb8623f0caf1034fc005cbf1c375b52bd241ac03a6097f47f8f5bebe4a`  
		Last Modified: Wed, 26 Jan 2022 07:09:59 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f47112e15cf1e76a8523b212f677adc2d250a7dfe6462a7af6419e38b6600b`  
		Last Modified: Wed, 26 Jan 2022 07:09:59 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063ac808e98463d36f7f6107482f64f5091038bc0cc34de6c66fe076f9ddcecd`  
		Last Modified: Wed, 26 Jan 2022 07:09:59 GMT  
		Size: 4.7 KB (4728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; 386

```console
$ docker pull postgres@sha256:595497934783e2abba617f97d7de23cff0f605698b7ac1451519a8b5f0694239
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (109967718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da04fa6e0368ad366ac622a13e48820532fb496d6f716befa9ebace56d3c7aea`
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
# Wed, 26 Jan 2022 20:40:37 GMT
ENV PG_MAJOR=11
# Wed, 26 Jan 2022 20:40:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Wed, 26 Jan 2022 20:40:37 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Wed, 26 Jan 2022 20:41:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 26 Jan 2022 20:41:08 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 26 Jan 2022 20:41:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 26 Jan 2022 20:41:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 26 Jan 2022 20:41:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 26 Jan 2022 20:41:11 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 26 Jan 2022 20:41:11 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Wed, 26 Jan 2022 20:41:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 20:41:12 GMT
STOPSIGNAL SIGINT
# Wed, 26 Jan 2022 20:41:12 GMT
EXPOSE 5432
# Wed, 26 Jan 2022 20:41:12 GMT
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
	-	`sha256:b098c68dcf3ef344b56bc43c23c23c82e6c49a1be2bb78d5e8e901165f076994`  
		Last Modified: Wed, 26 Jan 2022 21:11:19 GMT  
		Size: 74.1 MB (74051380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454e4b4379e15738b544597e345924b3d17b65c624973d5873570b3dad4ed04d`  
		Last Modified: Wed, 26 Jan 2022 21:11:02 GMT  
		Size: 8.3 KB (8329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a870a43160f1a24dcae647bb92948e51a7d0b54cb9997b9074296c28c9e03a49`  
		Last Modified: Wed, 26 Jan 2022 21:11:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8a9ebe2f996fdf468f1750fb6718330c06415f215aed4101f078bb27a6a67f`  
		Last Modified: Wed, 26 Jan 2022 21:11:02 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dffa480c56b15cdb2bf1662f7acab84c23b6836c8188b64a16e280da2ebd1c`  
		Last Modified: Wed, 26 Jan 2022 21:11:02 GMT  
		Size: 4.7 KB (4726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
