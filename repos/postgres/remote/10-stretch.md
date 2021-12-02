## `postgres:10-stretch`

```console
$ docker pull postgres@sha256:42556aa93c65b2dc262d01af75a57d8e5eeee95cb2702a1f8f8cb446b87940ff
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
$ docker pull postgres@sha256:3a3f1e96856acfb3b89ed21a613c046cf68d316c95133c45128789ba793f9b82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73177502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9429f74d34aa5b27edf9601c2ec14d288231e4bd5cc1a8f876543cc2a95a869`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:38 GMT
ADD file:2868c3af63afe6b8aadac07b8776e5468a3ed135fd84ad22df15e48f0610c7ba in / 
# Wed, 17 Nov 2021 02:22:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 21:57:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:57:36 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 05:25:58 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 05:26:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 05:26:26 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 05:26:26 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 05:26:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 05:26:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 05:26:43 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 05:35:11 GMT
ENV PG_MAJOR=10
# Tue, 30 Nov 2021 05:35:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 30 Nov 2021 05:35:12 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Tue, 30 Nov 2021 05:35:30 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 05:35:31 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 05:35:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 05:35:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 05:35:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 05:35:33 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 05:35:33 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Tue, 30 Nov 2021 05:35:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 30 Nov 2021 05:35:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 05:35:34 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 05:35:35 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 05:35:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:89166b5eeae47d8c878cb88f20cc67eda2a550a697f4be317c7b7abea566b76f`  
		Last Modified: Wed, 17 Nov 2021 02:29:32 GMT  
		Size: 22.5 MB (22527686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee3d94b0b2d5764212e2d7e629e9c3de7128ae21f9676d21cf8a4345241960`  
		Last Modified: Wed, 17 Nov 2021 22:03:44 GMT  
		Size: 4.5 MB (4503831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11070db47648b9388a78654fa06b64818270d1fffd11f47b2d0724a2d2b5743`  
		Last Modified: Wed, 17 Nov 2021 22:03:43 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e48ec3c101d1c9eb35ea72bf8bf7ea213f177f7b5ce712eccdb7d8981a543f9`  
		Last Modified: Tue, 30 Nov 2021 05:52:07 GMT  
		Size: 1.4 MB (1379405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a551d86500bc639cb60426e69632857adc622b692459f43201f680d8a75f2d7`  
		Last Modified: Tue, 30 Nov 2021 05:52:05 GMT  
		Size: 6.2 MB (6185285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21d1b96372a4d706f9a80b3973b4714d19fc5dfa05b2d4463d53f373ab5a3d5`  
		Last Modified: Tue, 30 Nov 2021 05:52:05 GMT  
		Size: 385.0 KB (385043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b707b86b0a88e71222795426118e56a17b9200c7548b14876c2436ed6cef80d0`  
		Last Modified: Tue, 30 Nov 2021 05:52:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dbb0367cc1887e834da274499f2b7fcb2e594f60d20a2511cecf2931e33cf1`  
		Last Modified: Tue, 30 Nov 2021 05:52:04 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19da2decf65774d6fbf6284efed21cb7dea63a4df83fa2e56d0555089e67210`  
		Last Modified: Tue, 30 Nov 2021 05:53:27 GMT  
		Size: 38.2 MB (38175691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbba3461cdb518ef7fcfbf07bce30cc2117602e62315add90ce920d1b7c2181`  
		Last Modified: Tue, 30 Nov 2021 05:53:17 GMT  
		Size: 8.1 KB (8081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d3b14ff30a5ceaed390e0f4230d6b74a7d467d0b0882b041eb3c6863550e85`  
		Last Modified: Tue, 30 Nov 2021 05:53:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99525a15a39c7a941c9e0762769a39ecffbe8ce223129cd900b9079a62415d4`  
		Last Modified: Tue, 30 Nov 2021 05:53:17 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d23efe643421c44a4c2b42b455c2803d0a151adaf178b2e96faaa5e45f4926`  
		Last Modified: Tue, 30 Nov 2021 05:53:17 GMT  
		Size: 4.7 KB (4727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254c181a9bc7764c9a8a857874c958e173c8e4bb4db7d3b67acb2248539b0544`  
		Last Modified: Tue, 30 Nov 2021 05:53:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:b765fdd7b894f852e370d7079a584f653f517ef51571fcdae7b24d9872a8b8db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70230670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:398e9e418bdc3cc4738702cb8cd49c3bd94e6c3bed595cb363a91dbf234a4e0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 02 Dec 2021 02:57:55 GMT
ADD file:a1e328a7ceac3e567d9b78728b38c24f0199a7765deee05ba8115785a892b58f in / 
# Thu, 02 Dec 2021 02:57:56 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:26:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 08:26:55 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 02 Dec 2021 08:26:56 GMT
ENV GOSU_VERSION=1.14
# Thu, 02 Dec 2021 08:27:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 02 Dec 2021 08:27:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 02 Dec 2021 08:27:50 GMT
ENV LANG=en_US.utf8
# Thu, 02 Dec 2021 08:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 08:28:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 02 Dec 2021 08:28:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 02 Dec 2021 09:17:37 GMT
ENV PG_MAJOR=10
# Thu, 02 Dec 2021 09:17:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Thu, 02 Dec 2021 09:17:38 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Thu, 02 Dec 2021 09:43:33 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 02 Dec 2021 09:43:36 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 02 Dec 2021 09:43:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 02 Dec 2021 09:43:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 02 Dec 2021 09:43:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 02 Dec 2021 09:43:40 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 02 Dec 2021 09:43:40 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Thu, 02 Dec 2021 09:43:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 02 Dec 2021 09:43:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 09:43:43 GMT
STOPSIGNAL SIGINT
# Thu, 02 Dec 2021 09:43:43 GMT
EXPOSE 5432
# Thu, 02 Dec 2021 09:43:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6213aa8d791a7975f08a10bcacb7d9ef2d07474b772a2fe57ff37c4b0d47b28a`  
		Last Modified: Thu, 02 Dec 2021 03:15:59 GMT  
		Size: 21.2 MB (21203460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913f1c876703293ef5eae9131b972093f1c34712ea17fbbe31dda31f5c3e9c0f`  
		Last Modified: Thu, 02 Dec 2021 10:19:41 GMT  
		Size: 4.2 MB (4239302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10f1250dd99b3e36d245ab86fa2725737a96806e76525d81c1b3041a847d0b1`  
		Last Modified: Thu, 02 Dec 2021 10:19:38 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b10ebdde8c7786ff94f89a7c60484f69fef18f3725f301999097dfce3cf3b4`  
		Last Modified: Thu, 02 Dec 2021 10:19:38 GMT  
		Size: 1.3 MB (1344273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f398500633ceb3cf3841b9dc3fa07c4c1a7464be5a5a624619161844c67d55`  
		Last Modified: Thu, 02 Dec 2021 10:19:40 GMT  
		Size: 6.2 MB (6185675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e92443232f77b9ecda0a2c04dbc961034c17fecdfb0c2e00f4b546f980c80e3`  
		Last Modified: Thu, 02 Dec 2021 10:19:36 GMT  
		Size: 385.1 KB (385071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16588a6aa38d1c629c69c175cc7a99904c813960ff4a8ed3bfc7663595c623c`  
		Last Modified: Thu, 02 Dec 2021 10:19:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b9c1e6b3b638ad02886239e2d41b70d7192613762a4444115331b0538f3e95`  
		Last Modified: Thu, 02 Dec 2021 10:19:35 GMT  
		Size: 5.3 KB (5345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8254fc997416b07a3bb01dfa07183815cead1a64c2ade89e37dbcb031a35faa`  
		Last Modified: Thu, 02 Dec 2021 10:21:29 GMT  
		Size: 36.9 MB (36852336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a64e64d21999762fc7859961795264551da61e78fc5299a70d457f0ffd2a54`  
		Last Modified: Thu, 02 Dec 2021 10:21:02 GMT  
		Size: 8.1 KB (8085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61adf92631de48b2159fd1b24ab5c7b93e7d82c9f9e94903e3f3f7ac73cf69d5`  
		Last Modified: Thu, 02 Dec 2021 10:21:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eb9615228a9d2671cf0869f7b8c854cbce4b68931f11e05822273a6b3186e5`  
		Last Modified: Thu, 02 Dec 2021 10:21:02 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf47cf85566c3783a33b87016168c92205805c9e89c98558abea01aa6dce4830`  
		Last Modified: Thu, 02 Dec 2021 10:21:02 GMT  
		Size: 4.7 KB (4725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f75f9de50c75a5b290642278232b54849f61ef9b4f59b4feecbaf6ce76e1b`  
		Last Modified: Thu, 02 Dec 2021 10:21:02 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:f65bbc770620f1b465deb4575667d19b3730cfdcf413b8d43f89eab755f96cee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66900610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0974993a4a51a524efc2b3586655d973ea08a6a458ae91a55d6037e18b016fc6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:05:31 GMT
ADD file:f28546ff6a3759d3a957c25d4310c3065e1367dff4ae304caae1cf1dc64d061d in / 
# Wed, 17 Nov 2021 02:05:32 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 20:15:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 20:15:48 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 09:36:26 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 09:36:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 09:37:13 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 09:37:14 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 09:37:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 09:37:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 09:37:36 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 10:27:13 GMT
ENV PG_MAJOR=10
# Tue, 30 Nov 2021 10:27:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 30 Nov 2021 10:27:14 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Tue, 30 Nov 2021 10:49:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 10:49:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 10:49:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 10:49:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 10:49:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 10:49:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 10:50:00 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Tue, 30 Nov 2021 10:50:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 30 Nov 2021 10:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 10:50:02 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 10:50:02 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 10:50:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:614e23553da11f1294dc969bcab416c9f981794bdbaee5641335a222730c63b2`  
		Last Modified: Wed, 17 Nov 2021 02:22:41 GMT  
		Size: 19.3 MB (19316397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2effe6a5f16302abc8031470eb48915a81617487a7cd06cf52b124ab1002c8fb`  
		Last Modified: Wed, 17 Nov 2021 22:20:28 GMT  
		Size: 3.9 MB (3875425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670859d248795266b6fcb5b5607b9fcbc56b555701abde40671010685985c17f`  
		Last Modified: Wed, 17 Nov 2021 22:20:25 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5cef825a5bdb6d9d0b514ff71911ebbc21ff0d7e8fa41f4adc5a7703649d1d`  
		Last Modified: Tue, 30 Nov 2021 12:17:07 GMT  
		Size: 1.3 MB (1335890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9deff4a6a0f4977c3df43dacb8403dba26757e1eafbfc2118f9aa6cb13fdb94`  
		Last Modified: Tue, 30 Nov 2021 12:17:09 GMT  
		Size: 6.2 MB (6185633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb78a400d60c6dd6f3663e8f5791a763c44a63f04cc2ae284c859da6e1bbd99b`  
		Last Modified: Tue, 30 Nov 2021 12:17:05 GMT  
		Size: 379.2 KB (379188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03780188e28825795488afc3dbdb645d03dbbe7b143bae4784460d96b7b0b314`  
		Last Modified: Tue, 30 Nov 2021 12:17:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27d85d8b3265729e4bef90d9b10463f843f9e84cab936f0d42c14795e81b30c`  
		Last Modified: Tue, 30 Nov 2021 12:17:05 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46eac680a5e30505814264a596b41b7f7ea67100e9e276db8b7e26b2a4fd7f6`  
		Last Modified: Tue, 30 Nov 2021 12:19:52 GMT  
		Size: 35.8 MB (35787531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d5fc70314adcf2662cb54e4fb353a0bfad441f5ccc2aa61bdc7f0c2ac714db`  
		Last Modified: Tue, 30 Nov 2021 12:19:26 GMT  
		Size: 8.1 KB (8077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d420543b4108f5c388778f362d2cc1216027c1e532f7912291e2d5277249e7b2`  
		Last Modified: Tue, 30 Nov 2021 12:19:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e646e32fd119cd70b1da48a4308f8a71102a60eccca277dc60b4f819bbc1b8`  
		Last Modified: Tue, 30 Nov 2021 12:19:26 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cf5b0c83fd0df337a5cc19bd65d76b18f1daf027a1d7532a71a8db436168dd`  
		Last Modified: Tue, 30 Nov 2021 12:19:26 GMT  
		Size: 4.7 KB (4724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da93faa600ad9053333c29f1678973befea49ced504fbab8c00fe1c4d8ae328b`  
		Last Modified: Tue, 30 Nov 2021 12:19:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:68205c86d1aee461b9c2089e0571053c317fa7e8dda8f7e3a50f3bff6d2d1f19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69110681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cce39d957257ba2971fc062e43105dd5d5b63f8451526899b706963938cfb6cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 02 Dec 2021 08:10:23 GMT
ADD file:d9d01d3468e590cea0e2803b24fa9d34ca1d3eb31b517a5a0edf081f85e7dcc1 in / 
# Thu, 02 Dec 2021 08:10:23 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:24:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 14:24:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 02 Dec 2021 14:24:53 GMT
ENV GOSU_VERSION=1.14
# Thu, 02 Dec 2021 14:25:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 02 Dec 2021 14:25:12 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 02 Dec 2021 14:25:13 GMT
ENV LANG=en_US.utf8
# Thu, 02 Dec 2021 14:25:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:25:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 02 Dec 2021 14:25:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 02 Dec 2021 14:35:44 GMT
ENV PG_MAJOR=10
# Thu, 02 Dec 2021 14:35:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Thu, 02 Dec 2021 14:35:45 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Thu, 02 Dec 2021 14:44:24 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 02 Dec 2021 14:44:25 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 02 Dec 2021 14:44:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 02 Dec 2021 14:44:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 02 Dec 2021 14:44:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 02 Dec 2021 14:44:29 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 02 Dec 2021 14:44:31 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:44:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 02 Dec 2021 14:44:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 14:44:33 GMT
STOPSIGNAL SIGINT
# Thu, 02 Dec 2021 14:44:34 GMT
EXPOSE 5432
# Thu, 02 Dec 2021 14:44:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:99dcd33b7a52fa23a15c1dc3456487807f7ad0f48f3df675dc13490656cc96f9`  
		Last Modified: Thu, 02 Dec 2021 08:44:55 GMT  
		Size: 20.4 MB (20389365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f4e0a897ff7d8dfcbe3ebe4a891caa5e91281627586e8d4e0ba65fca20064`  
		Last Modified: Thu, 02 Dec 2021 14:58:38 GMT  
		Size: 3.9 MB (3890683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e4006bd82ee6a2e27a6d841e437077daa7202a8847fbca466f9f6561dc5322`  
		Last Modified: Thu, 02 Dec 2021 14:58:36 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef5686a034a22c158862ab36d94a9e9352929f2824c0974089da35ab58e2fca`  
		Last Modified: Thu, 02 Dec 2021 14:58:36 GMT  
		Size: 1.3 MB (1307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b36de2354f710c3cb7df0985cfe76bb9345dc93530826ffdb57279eb18a831`  
		Last Modified: Thu, 02 Dec 2021 14:58:36 GMT  
		Size: 6.2 MB (6182382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aa3a5a53efc3ef238a0f8ebd180ca406afe7c11f2dbd4dc4ae449f36ebb1d9`  
		Last Modified: Thu, 02 Dec 2021 14:58:34 GMT  
		Size: 173.4 KB (173393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4a4b5f9f5e989af72c0c52e177a4673f3a011cd4f626d62c59dbecfa702381`  
		Last Modified: Thu, 02 Dec 2021 14:58:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60555f757ad0ac1d25a58699559c20e5bb454774cf10a3fa887107d5fa344615`  
		Last Modified: Thu, 02 Dec 2021 14:58:34 GMT  
		Size: 5.3 KB (5316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f90b67eb7d7f48faa2d14eadc02709e334a2fd5424cd3807eb959fd64b42978`  
		Last Modified: Thu, 02 Dec 2021 14:59:26 GMT  
		Size: 37.1 MB (37146850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836a874602ab375ba7455dc26874e1b769246823371e90943ac670b7240557e4`  
		Last Modified: Thu, 02 Dec 2021 14:59:18 GMT  
		Size: 8.1 KB (8077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd42f72cfa0cc9d936a1a3b7ee5022abbcdf0ae9b5dc3b88a503e13f571e387f`  
		Last Modified: Thu, 02 Dec 2021 14:59:18 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc71ea0cd3da25e16fd6be82031fe4ad11acea200d4b0358e8e98970dd81153`  
		Last Modified: Thu, 02 Dec 2021 14:59:18 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac1e65a6c970162551e8f65239bdbb16e0d0d215c49824ab96f01c8b32d093d`  
		Last Modified: Thu, 02 Dec 2021 14:59:18 GMT  
		Size: 4.7 KB (4728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa0992f00da17df9e24f94a30a6706fc225ba23af29ac55ebad69e3ebedee6a`  
		Last Modified: Thu, 02 Dec 2021 14:59:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; 386

```console
$ docker pull postgres@sha256:0da032507a482f1033ea37975a43c2987a91ba7692bb7e736f07560ead4066ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74339240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ac25a767c15852cd3056120a1568afd824d428f66a222f7cd0d3c0e0e2e866`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:36 GMT
ADD file:3c9c1d0f88db0341cbe43b594cf6d2d865e39d9518b8e2b124cb9736bebe18f3 in / 
# Wed, 17 Nov 2021 02:42:37 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 14:53:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 14:54:00 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 03:57:13 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 03:57:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 03:57:36 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 03:57:36 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 03:57:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 03:57:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 03:57:51 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 04:16:28 GMT
ENV PG_MAJOR=10
# Tue, 30 Nov 2021 04:16:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 30 Nov 2021 04:16:28 GMT
ENV PG_VERSION=10.19-1.pgdg90+1
# Tue, 30 Nov 2021 04:16:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 04:16:57 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 04:16:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 04:16:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 04:16:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 04:17:00 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 04:17:00 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Tue, 30 Nov 2021 04:17:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 30 Nov 2021 04:17:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 04:17:02 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 04:17:03 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 04:17:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d213b39bd355350279fd232f3eedd77a11f7fb2a3d5a0017357dd45fa88342d1`  
		Last Modified: Wed, 17 Nov 2021 02:52:49 GMT  
		Size: 23.2 MB (23156564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc08762ac2638fdc5d798ba8a717a91d7fbcd7421f6ec0f557c6d1eb6f03c0d`  
		Last Modified: Wed, 17 Nov 2021 15:24:32 GMT  
		Size: 4.8 MB (4811942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358db85f042b097401ff43f08eea1438a5b1bc968738ae1cfa437a21d436f9be`  
		Last Modified: Wed, 17 Nov 2021 15:24:31 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86c0ee4273eb6b713c1debc299c7d302bb29e45f1a192ee6aabcebb4635050`  
		Last Modified: Tue, 30 Nov 2021 04:47:41 GMT  
		Size: 1.3 MB (1347275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd466c9fb1a48aca5f4a766f5caade3755ca75146d6bda121e30c5fc52f39c3`  
		Last Modified: Tue, 30 Nov 2021 04:47:41 GMT  
		Size: 6.2 MB (6185183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a368c593985ff88b2b23c18669f855caa928d32aba48b4e3bfd6e1e78a9d8b09`  
		Last Modified: Tue, 30 Nov 2021 04:47:39 GMT  
		Size: 393.3 KB (393334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a139a1de4c617e9683f6035bf8ab5e0ced6501dd7e4a15c8cc88b41b8b86b2eb`  
		Last Modified: Tue, 30 Nov 2021 04:47:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5751839c1edb4176c7478a91082aa9af772d520186d77b724011fce1f8c9848`  
		Last Modified: Tue, 30 Nov 2021 04:47:39 GMT  
		Size: 5.3 KB (5345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9979b98fe47dfaa8c17e3a31375b9233171f7111165f1c5d4a81a088cc88c514`  
		Last Modified: Tue, 30 Nov 2021 04:49:25 GMT  
		Size: 38.4 MB (38424397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48bb0eba0ed49d254fe0d195538436cb9ec265a349ca8d92f37957e861def75`  
		Last Modified: Tue, 30 Nov 2021 04:49:15 GMT  
		Size: 8.1 KB (8073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7281db5783a6830590ab32aaa93701034ed6b0ebce6aff9a17dc15f850a41060`  
		Last Modified: Tue, 30 Nov 2021 04:49:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374645a0d2d3f4c54243b1a8fab19f6a1978b7eedcee7e2b1c52c7a1cc5008e4`  
		Last Modified: Tue, 30 Nov 2021 04:49:15 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b8712858a3d61e1af06002bc11aef7408ec01b312228b439ed2ff8d74f339f`  
		Last Modified: Tue, 30 Nov 2021 04:49:15 GMT  
		Size: 4.7 KB (4725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86bfff882af3df787e98031646c26e994860978401e3a71287327b3db87ab88`  
		Last Modified: Tue, 30 Nov 2021 04:49:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
