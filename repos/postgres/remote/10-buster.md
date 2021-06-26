## `postgres:10-buster`

```console
$ docker pull postgres@sha256:1e5b9005e59c730a099b92e6cefcd15b9026b06dcc1f03582e6f4b38999f3191
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

### `postgres:10-buster` - linux; amd64

```console
$ docker pull postgres@sha256:801fcd44b714f3fa58d027da995773600c1f859fad13265ab6c14f5e19d64ee3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81508291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75528f27a248618a7c2f78448d407db7cd8070daa5418b4193f10802c07db2b8`
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
# Wed, 23 Jun 2021 14:14:31 GMT
ENV PG_MAJOR=10
# Wed, 23 Jun 2021 14:14:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 23 Jun 2021 14:14:31 GMT
ENV PG_VERSION=10.17-1.pgdg100+1
# Wed, 23 Jun 2021 14:14:47 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 14:14:48 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 14:14:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 14:14:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 14:14:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 14:14:50 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 14:14:51 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 14:14:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 14:14:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 14:14:52 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 14:14:52 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 14:14:52 GMT
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
	-	`sha256:62f4dfd10e98d56568d258842b986bc2bc0ffc0bcc2e5478623247f7a5d512da`  
		Last Modified: Wed, 23 Jun 2021 14:22:39 GMT  
		Size: 40.4 MB (40389356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72731c2559d0fe6fe274a9922ce7f3af23ec96921abc2cbc0f3c769af2897cb3`  
		Last Modified: Wed, 23 Jun 2021 14:22:28 GMT  
		Size: 8.1 KB (8077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e554674c130a68da8da35506e41dc9a1860ef24fe58ee0f9ee98474c628b3d2`  
		Last Modified: Wed, 23 Jun 2021 14:22:28 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2e5894ef8c6f2336dbd237bf98cd1349774e0da7ef2098afb44ef2d1b8100d`  
		Last Modified: Wed, 23 Jun 2021 14:22:28 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a8b3f16bc1c59856381aed75f2dcb59bf4e34ed38b76293784892f266cb788`  
		Last Modified: Wed, 23 Jun 2021 14:22:28 GMT  
		Size: 4.4 KB (4400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74613c3cae025a1fd393094d95154cd51ce3aa9a919753b5eced7a2a3ddfcb25`  
		Last Modified: Wed, 23 Jun 2021 14:22:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-buster` - linux; arm variant v5

```console
$ docker pull postgres@sha256:bb20f213b5c6332f1a88abd617c7e5bb2fec8128d34883bab919899ebdfc3f48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77218430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65027832b56d4efaf90e8a637587e0b4df952956c1059534e1c458bf319405bc`
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
# Wed, 23 Jun 2021 11:10:30 GMT
ENV PG_MAJOR=10
# Wed, 23 Jun 2021 11:10:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 23 Jun 2021 11:10:31 GMT
ENV PG_VERSION=10.17-1.pgdg100+1
# Wed, 23 Jun 2021 11:33:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 11:33:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 11:33:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 11:33:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 11:33:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 11:33:59 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 11:33:59 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 11:34:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 11:34:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 11:34:01 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 11:34:02 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 11:34:02 GMT
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
	-	`sha256:905397396f3da1bb4d106cd427596cfdcfe4d3ec11c5f0d82bfc47bca1542c2c`  
		Last Modified: Wed, 23 Jun 2021 12:58:23 GMT  
		Size: 38.7 MB (38739027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54363ad9f2ed91f092d7121c8f7434a81736839b2331b5b54702a9d6cff73caf`  
		Last Modified: Wed, 23 Jun 2021 12:58:04 GMT  
		Size: 8.1 KB (8083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317731bf8fe15e0e786278546f8a1e52f96a77418230666938c0894374db350d`  
		Last Modified: Wed, 23 Jun 2021 12:58:04 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2b4e8395df1720abb85765682f3483013f414912bfa38bb59756fab024059c`  
		Last Modified: Wed, 23 Jun 2021 12:58:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b67be663f07cfcc41b6b067d05399ad3bc04cd176575cd1e999506a797f5fae`  
		Last Modified: Wed, 23 Jun 2021 12:58:04 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b0cad1ced10d1822fa427061f3667eb5317eb29a4b4318b0a43d0303231fac`  
		Last Modified: Wed, 23 Jun 2021 12:58:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-buster` - linux; arm variant v7

```console
$ docker pull postgres@sha256:a29307be5f4dbb8370b92063df618ff8d4fd7478d8e205ea35479f18470510c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73610848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f753afd9afabc31b9a4b9c9ae40dd98e19892536ae1860ee4e120dd5c18817`
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
# Wed, 23 Jun 2021 21:10:30 GMT
ENV PG_MAJOR=10
# Wed, 23 Jun 2021 21:10:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 23 Jun 2021 21:10:31 GMT
ENV PG_VERSION=10.17-1.pgdg100+1
# Wed, 23 Jun 2021 21:32:08 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 21:32:10 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 21:32:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 21:32:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 21:32:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 21:32:14 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 21:32:15 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 21:32:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 21:32:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 21:32:17 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 21:32:18 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 21:32:18 GMT
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
	-	`sha256:c4a489a553ae9ca09c42e9f758e38f8465be2642efc17a2a0babc35a5dc37ed3`  
		Last Modified: Wed, 23 Jun 2021 22:53:39 GMT  
		Size: 37.6 MB (37644402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763c5bbb7370131a5f5e3365ba8a247460c91c3729b134c520badc6ba6776447`  
		Last Modified: Wed, 23 Jun 2021 22:53:11 GMT  
		Size: 8.1 KB (8077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc4f4a050128d94b8c9bf7cc318bf2fd40403d112f5cdb6af4ab9b919458208`  
		Last Modified: Wed, 23 Jun 2021 22:53:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35a3d491b8c8c422d96497a4f712498a140f9e68103c2e6941bd135b6c1c856`  
		Last Modified: Wed, 23 Jun 2021 22:53:11 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56968a21642a0f8b9d3b085b74d45fc5eee2a2ab411be583b5b4818b5182001`  
		Last Modified: Wed, 23 Jun 2021 22:53:11 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de0f1929f246f30dd44b49de73f12ec3e0463a53bbaf55a8a4ce58f9ca92e9e`  
		Last Modified: Wed, 23 Jun 2021 22:53:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-buster` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:546205cc4cf5106a51d37b22c0869293a70a605b796d3d18740c3d052c5404fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.9 MB (79903848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcf9b144097b49c8d0f5620f44ddff9b737418ac20a138665cca9dbcebc8bab`
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
# Wed, 23 Jun 2021 08:19:18 GMT
ENV PG_MAJOR=10
# Wed, 23 Jun 2021 08:19:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 23 Jun 2021 08:19:18 GMT
ENV PG_VERSION=10.17-1.pgdg100+1
# Wed, 23 Jun 2021 08:19:34 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 08:19:35 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 08:19:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 08:19:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 08:19:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 08:19:37 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 08:19:37 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 08:19:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 08:19:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 08:19:38 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 08:19:38 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 08:19:38 GMT
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
	-	`sha256:4158ca14d02ecf4460db5eb8ff13145e2e7c3b068ed8aee4fe8b766901515191`  
		Last Modified: Wed, 23 Jun 2021 08:45:56 GMT  
		Size: 40.1 MB (40091740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73aeae08f349cbdacd10703013c5c2a60c9ab918b3261640e4ffaaacb53f472c`  
		Last Modified: Wed, 23 Jun 2021 08:45:46 GMT  
		Size: 8.1 KB (8076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56be0a88d6c1b190f5fb87938123c5a70cc46fe0b5588b84dd7b2afa7819e721`  
		Last Modified: Wed, 23 Jun 2021 08:45:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4616f778de9c39596c386cee1418e4ca80d00a887c08dfd457c1026d546caa09`  
		Last Modified: Wed, 23 Jun 2021 08:45:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ab8c47357970011d4f5efb2a4a18a934669f0ecd9b11981f3b1e39a85b1f5`  
		Last Modified: Wed, 23 Jun 2021 08:45:46 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018a99031da6147f959651a599002ddaa5b26984ca54a225be925859ff9e4a7`  
		Last Modified: Wed, 23 Jun 2021 08:45:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-buster` - linux; 386

```console
$ docker pull postgres@sha256:a70e90a853d4d3b79e635d48e03809904349809832042249bc1549c00b8a2b96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.7 MB (82733661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5efd1f17c1d963d4ea342d709c67573ad36e8554d721996ae85c644aed31ec3f`
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
# Wed, 23 Jun 2021 12:53:55 GMT
ENV PG_MAJOR=10
# Wed, 23 Jun 2021 12:53:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 23 Jun 2021 12:53:56 GMT
ENV PG_VERSION=10.17-1.pgdg100+1
# Wed, 23 Jun 2021 12:54:17 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 12:54:18 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 12:54:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 12:54:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 12:54:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 12:54:20 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 12:54:20 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 12:54:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 12:54:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 12:54:22 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 12:54:22 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 12:54:22 GMT
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
	-	`sha256:090d7ed2adc92e02248441f49776516601b96262ca57289ac0d982434b2b2384`  
		Last Modified: Wed, 23 Jun 2021 13:04:59 GMT  
		Size: 40.6 MB (40621979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8554256a18b3b1b944e2491c85d5966a84c487443ce2c9757f861a1f5ff7955`  
		Last Modified: Wed, 23 Jun 2021 13:04:46 GMT  
		Size: 8.1 KB (8075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8478af7054507b6817223ebe1200a3163da9644f62153196cadac2a0a610c03`  
		Last Modified: Wed, 23 Jun 2021 13:04:46 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666a9188cf2b72bfec96b141febeb4323e70ee803cd1af5e86c6573ebffdb3de`  
		Last Modified: Wed, 23 Jun 2021 13:04:46 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b1a602ed58600fd9593894024d3cf012192694567232e182c0cbbd8226a053`  
		Last Modified: Wed, 23 Jun 2021 13:04:46 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312bef82939adc2b89c5503a5fc4a169385b1c87047e0e94432ec33be59cb07f`  
		Last Modified: Wed, 23 Jun 2021 13:04:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-buster` - linux; mips64le

```console
$ docker pull postgres@sha256:31d545c3cd662ea9873fc61fca8eeca0c1938cefa0846a1136dd847fc7979b46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78649691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ecff0d22b4cddd0a562f78ea1d1499556be41dd45304aca5c90e923e521824a`
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
# Wed, 23 Jun 2021 08:40:17 GMT
ENV PG_MAJOR=10
# Wed, 23 Jun 2021 08:40:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 23 Jun 2021 08:40:18 GMT
ENV PG_VERSION=10.17-1.pgdg100+1
# Wed, 23 Jun 2021 09:16:12 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 09:16:15 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 09:16:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 09:16:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 09:16:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 09:16:19 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 09:16:20 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 09:16:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 09:16:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 09:16:22 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 09:16:23 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 09:16:23 GMT
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
	-	`sha256:d399194d4ec02c681948f9024133ae1abf70cd67a9cc4e8b39ed1fd06a64e737`  
		Last Modified: Wed, 23 Jun 2021 09:55:45 GMT  
		Size: 39.0 MB (38974962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb620d874b1e9c4fce7e37302c145cfbb70c60a14915f3f9f66d7856d186860`  
		Last Modified: Wed, 23 Jun 2021 09:55:11 GMT  
		Size: 8.1 KB (8079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2517d852c7e36a5a1a3f0e6d6fa954963c62cf4a440dc5ed6299af0691e1192`  
		Last Modified: Wed, 23 Jun 2021 09:55:11 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f3272fd6aeee7eb7b0a55d1c2ccb43ace1243587be964fa51c7defbf7eb2d7`  
		Last Modified: Wed, 23 Jun 2021 09:55:11 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768a2caccac55a304555692d3e28d5782e85d487cb95ebf543a653456d6040b1`  
		Last Modified: Wed, 23 Jun 2021 09:55:11 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0608ccbd015f2fc2457b1c095ea1533e137cb32a78637e06ebe980ed627d80`  
		Last Modified: Wed, 23 Jun 2021 09:55:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-buster` - linux; ppc64le

```console
$ docker pull postgres@sha256:befb4dc6e16ef754c668808411d979e1056b2b9ee5cceb20a548a2cd7e363331
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.6 MB (87585194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9f82ecc24cd86a39c7a392b5493955325a6f206029414f5504b78bf6d4415b`
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
# Fri, 25 Jun 2021 20:58:11 GMT
ENV PG_MAJOR=10
# Fri, 25 Jun 2021 20:58:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Fri, 25 Jun 2021 20:58:32 GMT
ENV PG_VERSION=10.17-1.pgdg100+1
# Fri, 25 Jun 2021 21:02:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 25 Jun 2021 21:03:18 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 25 Jun 2021 21:03:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 25 Jun 2021 21:03:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 25 Jun 2021 21:04:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 25 Jun 2021 21:04:30 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 25 Jun 2021 21:04:33 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 25 Jun 2021 21:04:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Jun 2021 21:04:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 21:05:02 GMT
STOPSIGNAL SIGINT
# Fri, 25 Jun 2021 21:05:12 GMT
EXPOSE 5432
# Fri, 25 Jun 2021 21:05:21 GMT
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
	-	`sha256:96cda481541f5c45473a454ee104374264796d37a40c1e22b019158a70d0eac8`  
		Last Modified: Fri, 25 Jun 2021 21:26:17 GMT  
		Size: 42.3 MB (42345324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a6d65896fb882d060f8c32cb964c3e8d4056a0556ff0d890097fd0d96b48de`  
		Last Modified: Fri, 25 Jun 2021 21:26:03 GMT  
		Size: 8.1 KB (8087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0740041c5242aedc6b945a71e39359fa94cfe970aafd5306af091f59c88087`  
		Last Modified: Fri, 25 Jun 2021 21:26:02 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2696b5dd975c435f42613d3f30af519e0150ddfc7bf7954b171267860a4f7c2`  
		Last Modified: Fri, 25 Jun 2021 21:26:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bdcfeb25b143b25679f8e2a53bcf3b9291dbd9f1ee8cde498e2cbe95188867`  
		Last Modified: Fri, 25 Jun 2021 21:26:02 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eb04c6614701bb79eb4ba55ff22ec685a26b5163b44164a61eb36b0bbb3542`  
		Last Modified: Fri, 25 Jun 2021 21:26:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-buster` - linux; s390x

```console
$ docker pull postgres@sha256:73109b33e07f76946ffe468b426331759efe32583bc8056865a1f00cb9132cb3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.9 MB (79932447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bc34c4e9522c903d3dfc7555ae9c87cff6728c0c15df792c565752f8e5fc068`
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
# Fri, 25 Jun 2021 23:14:27 GMT
ENV PG_MAJOR=10
# Fri, 25 Jun 2021 23:14:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Fri, 25 Jun 2021 23:14:27 GMT
ENV PG_VERSION=10.17-1.pgdg100+1
# Fri, 25 Jun 2021 23:22:12 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 25 Jun 2021 23:22:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 25 Jun 2021 23:22:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 25 Jun 2021 23:22:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 25 Jun 2021 23:22:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 25 Jun 2021 23:22:20 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 25 Jun 2021 23:22:20 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 25 Jun 2021 23:22:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 25 Jun 2021 23:22:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 25 Jun 2021 23:22:22 GMT
STOPSIGNAL SIGINT
# Fri, 25 Jun 2021 23:22:22 GMT
EXPOSE 5432
# Fri, 25 Jun 2021 23:22:22 GMT
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
	-	`sha256:bf3134d478aef1eba80323bd19b4118efa0f4bffb06a6a357525bafc5b847622`  
		Last Modified: Fri, 25 Jun 2021 23:35:49 GMT  
		Size: 40.3 MB (40279618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1337a8e747a680ad71579bb67967977f541953e902945c3321031a5349d86e2`  
		Last Modified: Fri, 25 Jun 2021 23:35:41 GMT  
		Size: 8.1 KB (8078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025a3db271bacb6bb40f32cae25c81b35965104710b396df2488a939b6cdac7c`  
		Last Modified: Fri, 25 Jun 2021 23:35:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c5c4d368bee1af66913af6b465c7e3c57f39159e0bdfc53c845bb83dd5e4df`  
		Last Modified: Fri, 25 Jun 2021 23:35:42 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cd1f0eb000966d57e9c60299b6ef6fd4c16f4f1a11617a2078b87d9adb72e3`  
		Last Modified: Fri, 25 Jun 2021 23:35:41 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5050de55b0ec673dd811663432c646ab2c001b036b7c542c871bb5e07a5e9fe`  
		Last Modified: Fri, 25 Jun 2021 23:35:42 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
