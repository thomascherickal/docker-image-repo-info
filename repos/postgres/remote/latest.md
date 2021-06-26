## `postgres:latest`

```console
$ docker pull postgres@sha256:c5943760916b897e73906d31b13236f6788376da64a2996c8944e6dbbbd418c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `postgres:latest` - linux; amd64

```console
$ docker pull postgres@sha256:90b8a9f0cc7aad1bd17e49c5b753cde29615229acbc6a350390ca1a788458a19
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114945994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed45d5bb6847268ddf4bb0948e5c4aabfc1dd794633f07a5f0ee8ea6bc40d484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 14:04:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 14:04:21 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 14:04:21 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 14:04:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 14:04:39 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 14:04:40 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 14:04:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 14:04:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 14:04:48 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 23 Jun 2021 14:04:48 GMT
ENV PG_MAJOR=13
# Wed, 23 Jun 2021 14:04:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 23 Jun 2021 14:04:49 GMT
ENV PG_VERSION=13.3-1.pgdg100+1
# Wed, 23 Jun 2021 14:05:20 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 14:05:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 14:05:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 14:05:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 14:05:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 14:05:27 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 14:05:27 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 14:05:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 14:05:28 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 14:05:28 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 14:05:28 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ca1d02c28c23d7be49ab7fa29a9098c72b5b0278224d0cfd8463165fc020e7`  
		Last Modified: Wed, 23 Jun 2021 14:20:17 GMT  
		Size: 4.2 MB (4179266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a756866b55651110c82d478a4d84c87f8f2b62fb031ceaa483ed725632ae48fc`  
		Last Modified: Wed, 23 Jun 2021 14:20:16 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c49e539e90787e170cab973c5c22d9ed6aa119b6df188a1fe3738e4d5c1dbf`  
		Last Modified: Wed, 23 Jun 2021 14:20:16 GMT  
		Size: 1.4 MB (1419447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664019fbcaffaad28bb7ddb8c63788fa416f47992e5d8ee69872ee167e030a4a`  
		Last Modified: Wed, 23 Jun 2021 14:20:16 GMT  
		Size: 8.0 MB (7965239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727aeee9c480a26388cd1b5781aca4ac09044c77e5de9eefd038ca89bc98fc45`  
		Last Modified: Wed, 23 Jun 2021 14:20:14 GMT  
		Size: 391.2 KB (391200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796589e6b2239c66f6436e8330d2b8ea31285ab58b50251f6fd64422497a91cd`  
		Last Modified: Wed, 23 Jun 2021 14:20:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6664992e747d54a74b2d7da818edb6b2247b86ad593f82ca66a85067edd18356`  
		Last Modified: Wed, 23 Jun 2021 14:20:13 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f933aa7ccec23f0b0486d841f2baf4624559113fc5221a075112e4dd00ede6f`  
		Last Modified: Wed, 23 Jun 2021 14:20:24 GMT  
		Size: 73.8 MB (73825906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b5e5d88b32df91401fa8f1ecec71316cdf3d0dd281b00fbac31f1b2295f9ba`  
		Last Modified: Wed, 23 Jun 2021 14:20:10 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a901b82e60049c0e54cafd93ebfe103561d5926942616f64120948e707d4f4e6`  
		Last Modified: Wed, 23 Jun 2021 14:20:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625fd35fd0f372ab6eb7c8ef40b1b320a62e001f9a097be469c2e339a0126d44`  
		Last Modified: Wed, 23 Jun 2021 14:20:10 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e37bf358a5d9064e9336b30b86a40b960ef7aba46de4cc6c85f46da3b3f36cc`  
		Last Modified: Wed, 23 Jun 2021 14:20:10 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v5

```console
$ docker pull postgres@sha256:59c930fb5ae0fa8d0717316923089f620f1f54db5271bb79c8f3aa9f4d5cb2d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.1 MB (109127722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1970ff9a99396c7500fb31e4ddc5d362f5f3dcab79d9afe3e3cce8e72c971bc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 09:03:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 09:03:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 09:03:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 09:03:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 09:04:02 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 09:04:03 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 09:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 09:04:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 09:04:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 23 Jun 2021 09:04:21 GMT
ENV PG_MAJOR=13
# Wed, 23 Jun 2021 09:04:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 23 Jun 2021 09:04:22 GMT
ENV PG_VERSION=13.3-1.pgdg100+1
# Wed, 23 Jun 2021 09:37:19 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 09:37:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 09:37:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 09:37:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 09:37:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 09:37:28 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 09:37:28 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 09:37:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 09:37:29 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 09:37:29 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 09:37:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9356c8baa044f7480447faf123a44ccf980ed1277a0ff93a70f66c95704e7a`  
		Last Modified: Wed, 23 Jun 2021 12:54:53 GMT  
		Size: 3.8 MB (3848044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b3eb986bc9a017407731daa3753ed16445168b35540175ed4ee9d4f897573c`  
		Last Modified: Wed, 23 Jun 2021 12:54:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f7375e504de712ccf6b2056b72f27a8aa247d3dd7e88ad0a974fdceedc6ed9`  
		Last Modified: Wed, 23 Jun 2021 12:54:51 GMT  
		Size: 1.4 MB (1378688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b784d9e578f1e0be44144c8b58fa9c5e8a1cf2c7e844d91de63b6f7ba7ba1aac`  
		Last Modified: Wed, 23 Jun 2021 12:54:54 GMT  
		Size: 8.0 MB (7965284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7527da1db9bae446e5e6842d6da43335a0e0d3c13f9125559bc75d5f68ffefd`  
		Last Modified: Wed, 23 Jun 2021 12:54:49 GMT  
		Size: 390.5 KB (390505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4472fb4db9958f51746527ae7653f5b01b5c6318179ee13f3e84937bb39ddcd4`  
		Last Modified: Wed, 23 Jun 2021 12:54:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285da736af3b37070c42ec800829c0da710ce92de67268750b8af18db0a81c11`  
		Last Modified: Wed, 23 Jun 2021 12:54:48 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3476e56d88218c670d30121411e8d604a09491c0859e93ae19d77178e9cf00f3`  
		Last Modified: Wed, 23 Jun 2021 12:55:16 GMT  
		Size: 70.6 MB (70647173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c82088df1e76c77a17f8ed7f228ffae7c9eb31f6735fdc62a5e59307b03600d`  
		Last Modified: Wed, 23 Jun 2021 12:54:46 GMT  
		Size: 9.3 KB (9348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce059c12947a1182ff9beae9ec1d4a2db7efbe1d83bcafc724be706edb768a3`  
		Last Modified: Wed, 23 Jun 2021 12:54:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bbc7464544e837aab4261e7e7a4a24888333f9e60e1dc9c52fb19cba46b68e`  
		Last Modified: Wed, 23 Jun 2021 12:54:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67f83e751b1f6710b5f0217aa7a0b3bb5a362ed3ad880a7838ccb02a69d98ed`  
		Last Modified: Wed, 23 Jun 2021 12:54:46 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v7

```console
$ docker pull postgres@sha256:4eb14343e14e6f7a4c2c0182e759f5ade8dce08ea82c0659a5accf31067700fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105201971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9b6bdacc6e9a0bf7dcd664e274d1da3cebd333f7c4d55f17d609952afa5f74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 19:01:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 19:01:46 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 19:01:46 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 19:02:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 19:02:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 19:02:28 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 19:02:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 19:02:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 19:02:42 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 23 Jun 2021 19:02:42 GMT
ENV PG_MAJOR=13
# Wed, 23 Jun 2021 19:02:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 23 Jun 2021 19:02:43 GMT
ENV PG_VERSION=13.3-1.pgdg100+1
# Wed, 23 Jun 2021 19:32:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 19:32:44 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 19:32:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 19:32:47 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 19:32:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 19:32:50 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 19:32:51 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 19:32:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 19:32:52 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 19:32:53 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 19:32:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13ca8def4a6313f4027cf9352c6336ff2be95e89fa76d54c6e63b53cab316ab`  
		Last Modified: Wed, 23 Jun 2021 22:49:11 GMT  
		Size: 3.5 MB (3481690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb4004b5245d11e7c5a1c6ed8cab4458a262875fa0d8f1375ee9a4fb8c4b22`  
		Last Modified: Wed, 23 Jun 2021 22:49:09 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c22ff2a3ac568bec7b813ad51cb4340b09233647364b1cc99279ed3c086aa9`  
		Last Modified: Wed, 23 Jun 2021 22:49:09 GMT  
		Size: 1.4 MB (1370461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca690d281cb117df09748dc9fb2cdee7e8a8b2d6d8403b0bba156997aff9daa4`  
		Last Modified: Wed, 23 Jun 2021 22:49:13 GMT  
		Size: 8.0 MB (7965235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dddc39957aa87a1c05c093fb232a77d29a40a0f1346f44ddc4732c9d9adf37c`  
		Last Modified: Wed, 23 Jun 2021 22:49:07 GMT  
		Size: 385.1 KB (385072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1eb1c6e497c7d81df62422319499884b90ed05a2c0065fc96ca86f95ca1f7b`  
		Last Modified: Wed, 23 Jun 2021 22:49:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae4e39e7d2e9166d3df56fad88a5f8ed32c3d1d59c0f9a008d254249f3fcc59`  
		Last Modified: Wed, 23 Jun 2021 22:49:07 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1de8a031e2982117871d8c0e87fc8d0800418ee227c1a36aee045783ff16488`  
		Last Modified: Wed, 23 Jun 2021 22:49:50 GMT  
		Size: 69.2 MB (69234378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43a346bf0d61366e6620b19932aa20184da6b6d596306a6a41f57525fecab36`  
		Last Modified: Wed, 23 Jun 2021 22:49:05 GMT  
		Size: 9.3 KB (9350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cbbf57e0bdd9018c3b3da6c2617e90bc2bf2cf3d5276f50ee50b71a23b0d1c`  
		Last Modified: Wed, 23 Jun 2021 22:49:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b17bea56c7426304d351e7297279f45d03693e5d18479b2b772bb6615dff1b`  
		Last Modified: Wed, 23 Jun 2021 22:49:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddbb0728cd33e09cae49efb2e19d04896aae84891bfe1c4c58cac049953afcd`  
		Last Modified: Wed, 23 Jun 2021 22:49:05 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:179c9da75dee161350afd9c3e50528855dc6ee7d5063028a39854a4eafa06cf4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.3 MB (111255840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24ddd78d62db61600c9dd3c64efa79bb2c7d906da1503a7b9255aafa39146d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 08:00:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 08:00:55 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 08:01:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 08:01:10 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 08:01:11 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 08:01:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:01:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 08:01:17 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 23 Jun 2021 08:01:17 GMT
ENV PG_MAJOR=13
# Wed, 23 Jun 2021 08:01:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 23 Jun 2021 08:01:18 GMT
ENV PG_VERSION=13.3-1.pgdg100+1
# Wed, 23 Jun 2021 08:01:38 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 08:01:39 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 08:01:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 08:01:40 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 08:01:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 08:01:41 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 08:01:41 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 08:01:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 08:01:42 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 08:01:42 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 08:01:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ac3c0fe3ab17bfa4c3c1f905b67e705dd622e5b719250a3707da3275f6427c`  
		Last Modified: Wed, 23 Jun 2021 08:43:51 GMT  
		Size: 4.2 MB (4170280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4262cf38624a63127b9f8a869b2008bbbc19d68f64ea18a57e1a571a2ac4758a`  
		Last Modified: Wed, 23 Jun 2021 08:43:50 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa7b7e739f9235bd376773e956230ce34be4fee1ac7515b4b061e692e5bcbbd`  
		Last Modified: Wed, 23 Jun 2021 08:43:50 GMT  
		Size: 1.4 MB (1354308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b13a00ff8f5091034119a7504c90c399e5a944d7a4046a7d1de913d3af5d07`  
		Last Modified: Wed, 23 Jun 2021 08:43:50 GMT  
		Size: 8.0 MB (7965162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6582bc95f89c2fffbd09f50933c184070070b2f05ec18079f9253705c81aec`  
		Last Modified: Wed, 23 Jun 2021 08:43:48 GMT  
		Size: 389.4 KB (389428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9731edaa8053d4c7628e5bac8a251b7afd2831aea1b9cf30a41521f2684fd9a4`  
		Last Modified: Wed, 23 Jun 2021 08:43:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234d2c24f1fc9041caf2d2a5c9adc28a2b7132cb90abcee81043b07965f747a`  
		Last Modified: Wed, 23 Jun 2021 08:43:48 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1f48b202f29ad475cacd4701c2c46ade4f64e73c664d4e32be426474dc7eef`  
		Last Modified: Wed, 23 Jun 2021 08:43:56 GMT  
		Size: 71.4 MB (71442583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f950a2de470c59f7b830c09ad984d733e07fa1495d332438e7acb6ddfe422528`  
		Last Modified: Wed, 23 Jun 2021 08:43:45 GMT  
		Size: 9.3 KB (9346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9c9a4ff023ad28cafcbe5d26e6514eae14b54e825709756197bd4877cd9aff`  
		Last Modified: Wed, 23 Jun 2021 08:43:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46951b2fbe4f35611bd81c16c7145a0656fab4d682f56c1a5a2c0f7a3cd0f986`  
		Last Modified: Wed, 23 Jun 2021 08:43:45 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa0ea7ec16980c2ab5c6a004d4518026f50ae7fed138cfadeedecb054a679e6`  
		Last Modified: Wed, 23 Jun 2021 08:43:45 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; 386

```console
$ docker pull postgres@sha256:535235d72c46d21ad46d031f1317ab4b007828ed6e31e3dbd14b935117b00019
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115617488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f26a694f14519d65bd0f36405170a9e7f6208a542aac03c83ac1633efd59603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:42:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 12:42:15 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 12:42:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 12:42:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 12:42:34 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 12:42:34 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 12:42:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:42:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 12:42:42 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 23 Jun 2021 12:42:42 GMT
ENV PG_MAJOR=13
# Wed, 23 Jun 2021 12:42:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 23 Jun 2021 12:42:43 GMT
ENV PG_VERSION=13.3-1.pgdg100+1
# Wed, 23 Jun 2021 12:43:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 12:43:08 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 12:43:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 12:43:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 12:43:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 12:43:11 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 12:43:11 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 12:43:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 12:43:12 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 12:43:12 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 12:43:12 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d337bf957c6df38741b5e40521c285e05cb0a4fd816152795b87aa2cdc9ea2`  
		Last Modified: Wed, 23 Jun 2021 13:02:23 GMT  
		Size: 4.5 MB (4543049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54cc579aaa5b03770d3c48db25d3ffdeaaccd803d4301f1120afa40a5d64b22`  
		Last Modified: Wed, 23 Jun 2021 13:02:22 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bdd37951abcf0b02b48d936a834ada8859fe9fd623192fe8e0df85688e9255`  
		Last Modified: Wed, 23 Jun 2021 13:02:22 GMT  
		Size: 1.4 MB (1389734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bbf616aa63c2f5bf47d917d0e45349c1f688153c7e29c959da5ede1b18fe5a1`  
		Last Modified: Wed, 23 Jun 2021 13:02:22 GMT  
		Size: 8.0 MB (7965148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fc6f51dc19366217065dc4f6e5ce427a203c41ef072f01925f93b9b75f7114`  
		Last Modified: Wed, 23 Jun 2021 13:02:19 GMT  
		Size: 398.4 KB (398415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde873e5ee045524fd61da906c5125589d516733bafbee8ea73fd7efeb52ca69`  
		Last Modified: Wed, 23 Jun 2021 13:02:20 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfdaf67c8697132188e6b434f5884800f0e7e7a581d4495cec6a0f78282473d`  
		Last Modified: Wed, 23 Jun 2021 13:02:19 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516534b8ab29c9f2be2293ef97c3efd8a75e616c15a9f14d4eae51930db79910`  
		Last Modified: Wed, 23 Jun 2021 13:02:33 GMT  
		Size: 73.5 MB (73504660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c614d532a6cd0cc5757288ba97eba1199133aca6e5bac08a9a3d4cf5b4db088a`  
		Last Modified: Wed, 23 Jun 2021 13:02:17 GMT  
		Size: 9.3 KB (9345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d07c8938026a404551eacd4ae79987d0282456835bd56a4746d9910d24c021f`  
		Last Modified: Wed, 23 Jun 2021 13:02:16 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ed3bc5f661b20dbc8b31c65990c3747568087aeca59ad6e96b56c9ca3035bc`  
		Last Modified: Wed, 23 Jun 2021 13:02:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9670242a6c41cd84b4cb2541ba3ece839ebf332eccc7ce72253f3e2167b0205`  
		Last Modified: Wed, 23 Jun 2021 13:02:16 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; mips64le

```console
$ docker pull postgres@sha256:d15baeb20c60939524ba568ad02fbb90d9b176c1a88e6b20fa841ab10f7736b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110526795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f12758e76260be5eeea7e62112b0314135024106138c12a4111046e633b80fa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:29 GMT
ADD file:ca8422268fc66c67d19fd3a33a14a9bd6280ef21404677767ffd561a8ecf6724 in / 
# Wed, 23 Jun 2021 00:09:30 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:07:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 06:07:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 06:07:52 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 06:08:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 06:08:37 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 06:08:38 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 06:08:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:08:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 06:08:55 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 23 Jun 2021 06:08:55 GMT
ENV PG_MAJOR=13
# Wed, 23 Jun 2021 06:08:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 23 Jun 2021 06:08:56 GMT
ENV PG_VERSION=13.3-1.pgdg100+1
# Wed, 23 Jun 2021 07:00:19 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 07:00:21 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 07:00:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 07:00:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 07:00:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 07:00:25 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 07:00:25 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 07:00:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 07:00:26 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 07:00:26 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 07:00:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4b9d1870c33c63bfde89c401b4af9582fbbff99d4036171a7a456706bf805d6d`  
		Last Modified: Wed, 23 Jun 2021 00:15:49 GMT  
		Size: 25.8 MB (25812890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b9f45668f5dba1f89a88d75532d997f704b8f769464a0bfbaa662ffb85706a`  
		Last Modified: Wed, 23 Jun 2021 09:51:59 GMT  
		Size: 4.2 MB (4182534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57d181d0449273d41f292099c8908fa1e590de468df4356159f256f862ab4aa`  
		Last Modified: Wed, 23 Jun 2021 09:51:55 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271861430458d9727e85f81467f609676e2191235050e7e05ee3dbfbf58a36fd`  
		Last Modified: Wed, 23 Jun 2021 09:51:56 GMT  
		Size: 1.3 MB (1307443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6f1e5acaef2e967799d79017cdc838479984be994c337a19bffa377c3a5450`  
		Last Modified: Wed, 23 Jun 2021 09:52:00 GMT  
		Size: 8.0 MB (7964686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04eb0ca08420b979cb523bcccb5ff64fb26a99d9d33fa5ac9a2ef45bebf96f4`  
		Last Modified: Wed, 23 Jun 2021 09:51:52 GMT  
		Size: 389.3 KB (389337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ecd0ace3f5fc0389312e3e1e38e5e20f2204fb13ea29b111bc261a7af50309f`  
		Last Modified: Wed, 23 Jun 2021 09:51:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d66c891c30bea68bea297a0c3205ab50c3a6377dc478f308efce77fc10b6eb8`  
		Last Modified: Wed, 23 Jun 2021 09:51:52 GMT  
		Size: 3.1 KB (3053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab64a4b5f8721467fccf2086d67cadd29f45b37581f2ab01fb443a6c78efec`  
		Last Modified: Wed, 23 Jun 2021 09:52:40 GMT  
		Size: 70.9 MB (70850910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a817758af4b1a063c7ac006e00a9b3deb50ab7242526001d1b7b6a23fb7a1f`  
		Last Modified: Wed, 23 Jun 2021 09:51:49 GMT  
		Size: 9.4 KB (9352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a169c5d71ecf3db49f0d6ae59400b08553a3d7362411fc7cb40f99e0de1abcd`  
		Last Modified: Wed, 23 Jun 2021 09:51:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed5ae7fa5df1774b816327ae2f96b071323978e9d20f6858eca78c8adc80aec`  
		Last Modified: Wed, 23 Jun 2021 09:51:49 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3775f67b98129f04e9da07df2357068edef698520f21090d5247d88c26996fcb`  
		Last Modified: Wed, 23 Jun 2021 09:51:50 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; ppc64le

```console
$ docker pull postgres@sha256:0a1bd233db593b1c1bdf5e54e1f9eb9a1e1e46a5da0654b3b737fc2663b9af3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122208796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8e77de8f09918a23aea24ec246fabbf70e322a6f47c4b219b01cad2fa2b637`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 20:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 20:17:50 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 25 Jun 2021 20:17:55 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Jun 2021 20:18:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Jun 2021 20:19:13 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 25 Jun 2021 20:19:17 GMT
ENV LANG=en_US.utf8
# Fri, 25 Jun 2021 20:19:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 20:19:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Jun 2021 20:20:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Fri, 25 Jun 2021 20:20:06 GMT
ENV PG_MAJOR=13
# Fri, 25 Jun 2021 20:20:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 25 Jun 2021 20:20:12 GMT
ENV PG_VERSION=13.3-1.pgdg100+1
# Fri, 25 Jun 2021 20:21:42 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 25 Jun 2021 20:21:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 25 Jun 2021 20:22:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 25 Jun 2021 20:22:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 25 Jun 2021 20:22:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 25 Jun 2021 20:22:26 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 25 Jun 2021 20:22:29 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 25 Jun 2021 20:22:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 20:22:38 GMT
STOPSIGNAL SIGINT
# Fri, 25 Jun 2021 20:22:43 GMT
EXPOSE 5432
# Fri, 25 Jun 2021 20:22:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ea4be8d2b0973496bdf27a37866d300e573d62260959451dbe33029b47247e`  
		Last Modified: Fri, 25 Jun 2021 21:24:19 GMT  
		Size: 5.0 MB (4967501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbd8f4a01c8d204abe8160a2f2c361c64778d4921448ed1ebad3e705f7c307b`  
		Last Modified: Fri, 25 Jun 2021 21:24:16 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15c0bf2698f8ab4d43abcd074df35f06772fac34daf625cee5e7271b1706496`  
		Last Modified: Fri, 25 Jun 2021 21:24:16 GMT  
		Size: 1.3 MB (1338177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf35048c33cefcbed2d03927daccbcf618126ca68380d72cd6615a27ea82cfe2`  
		Last Modified: Fri, 25 Jun 2021 21:24:17 GMT  
		Size: 8.0 MB (7965501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceeb5abbd9fc69dbea44543f61a97c4828213a4b4466119771b57d7d9df993b`  
		Last Modified: Fri, 25 Jun 2021 21:24:14 GMT  
		Size: 397.1 KB (397108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f58c477d0109e843231139a52eabff989e09316c9b40b5e735718b4c1dc7401`  
		Last Modified: Fri, 25 Jun 2021 21:24:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0c4f85c860edeb4ebed04c54c52256d5529843451fb8291748f36293f62ec1`  
		Last Modified: Fri, 25 Jun 2021 21:24:09 GMT  
		Size: 3.1 KB (3052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d8ee32dde84a378212d1055a4fa6b271065b8ee70abfe26284e74550ae1fca`  
		Last Modified: Fri, 25 Jun 2021 21:24:19 GMT  
		Size: 77.0 MB (76967782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cc07a1519e27b1a96db5b2d3fb8b88cd93a773ec2391a156453edeb111e067`  
		Last Modified: Fri, 25 Jun 2021 21:24:04 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8ad279e41e564c181487d43dbf435816f0c3504d23cf698509cd9cb91ac5e9`  
		Last Modified: Fri, 25 Jun 2021 21:24:04 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73957f06aa0d269f82ce1c0d5698dce7f59c780504c7045e87aa22c941d080ed`  
		Last Modified: Fri, 25 Jun 2021 21:24:04 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066a1a07e2b1760c411f515a4b85662a29d1db2b70bb79b43860386d154a3dd2`  
		Last Modified: Fri, 25 Jun 2021 21:24:04 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; s390x

```console
$ docker pull postgres@sha256:7fe4874a406e3fe2e88f7f64e0d70d1e3fa17eb6d6e94a3901c6f8995d6f26d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113255155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fac1eb94de72628a360b99f8034a1c1d5138a80c5eb22670ccc4035ef18218f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:28 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Tue, 22 Jun 2021 23:42:29 GMT
CMD ["bash"]
# Fri, 25 Jun 2021 22:37:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 25 Jun 2021 22:37:29 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 25 Jun 2021 22:37:29 GMT
ENV GOSU_VERSION=1.12
# Fri, 25 Jun 2021 22:37:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 25 Jun 2021 22:37:46 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 25 Jun 2021 22:37:47 GMT
ENV LANG=en_US.utf8
# Fri, 25 Jun 2021 22:37:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 25 Jun 2021 22:37:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 25 Jun 2021 22:37:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Fri, 25 Jun 2021 22:37:55 GMT
ENV PG_MAJOR=13
# Fri, 25 Jun 2021 22:37:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 25 Jun 2021 22:37:55 GMT
ENV PG_VERSION=13.3-1.pgdg100+1
# Fri, 25 Jun 2021 22:47:49 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 25 Jun 2021 22:47:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 25 Jun 2021 22:47:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 25 Jun 2021 22:47:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 25 Jun 2021 22:47:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 25 Jun 2021 22:47:58 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 25 Jun 2021 22:47:58 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 25 Jun 2021 22:47:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 22:47:59 GMT
STOPSIGNAL SIGINT
# Fri, 25 Jun 2021 22:47:59 GMT
EXPOSE 5432
# Fri, 25 Jun 2021 22:48:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45236a7a815c299938884a1abcdc81cbfa8085f54efd5ec839b4560573a0f008`  
		Last Modified: Fri, 25 Jun 2021 23:34:44 GMT  
		Size: 4.1 MB (4060133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a914886d85d6e360629962b1a9e0b531599bf28b9606132716c64c6b88ddea`  
		Last Modified: Fri, 25 Jun 2021 23:34:43 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a5a54336f7f9a6056692a515b36850ac79f884c684e52c68cd8bb3786c487`  
		Last Modified: Fri, 25 Jun 2021 23:34:43 GMT  
		Size: 1.4 MB (1406192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb938832b5048d8a538120ba71c7e98bd4d4772206b8651945c487032e29920`  
		Last Modified: Fri, 25 Jun 2021 23:34:43 GMT  
		Size: 8.0 MB (8019443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a49ec12331a0cae0075cbac941b0f3a4ed888e13802fb9436fb6aea4c05734`  
		Last Modified: Fri, 25 Jun 2021 23:34:41 GMT  
		Size: 388.4 KB (388407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cacd4ad240e0c10577cdaa6c5f85091697e3cbebf40d11b0cd23658e8b4a4d`  
		Last Modified: Fri, 25 Jun 2021 23:34:41 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d59609808ab31ff1ca131fb77aed91f6352bf4c62d7ce37734d6a8b1785ce69`  
		Last Modified: Fri, 25 Jun 2021 23:34:41 GMT  
		Size: 3.1 KB (3052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c643b9fb1bc011a9cd84331a0d80830b2df1526c81673783855e62ef4a2c92c`  
		Last Modified: Fri, 25 Jun 2021 23:34:50 GMT  
		Size: 73.6 MB (73601177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca62fcb444312d1724818c61b32afea0484da47fe34af3ba482c68aacd2853f`  
		Last Modified: Fri, 25 Jun 2021 23:34:40 GMT  
		Size: 9.3 KB (9348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe61672b5928cf35c06928babd5316ab4512d2596db069d05c4923f8b04d7da2`  
		Last Modified: Fri, 25 Jun 2021 23:34:40 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b4c83a0b52be8493d7bd37618e05ce77b687e31eecab7c4d58a354e669ef87`  
		Last Modified: Fri, 25 Jun 2021 23:34:40 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab2686038a0ec5d84bbc92bea684005bfc82ea25ae2c714097027ab2ad024eb`  
		Last Modified: Fri, 25 Jun 2021 23:34:40 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
