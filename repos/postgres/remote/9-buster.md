## `postgres:9-buster`

```console
$ docker pull postgres@sha256:c8a118b2f284e29baf1905acbb497a035ddb31044008046696403b0885ddc0dc
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

### `postgres:9-buster` - linux; amd64

```console
$ docker pull postgres@sha256:2b76e4befa8ab09c29d987a4d888df1b676faaeed38746206bf3252936553114
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81867906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51f6af954d8e73c49c678d4000d2e6b0a7dcebc9b76e32cd70ca0cc7ea85bd5e`
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
# Mon, 12 Jul 2021 22:21:30 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Mon, 12 Jul 2021 22:25:07 GMT
ENV PG_MAJOR=9.6
# Mon, 12 Jul 2021 22:25:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Mon, 12 Jul 2021 22:25:07 GMT
ENV PG_VERSION=9.6.22-1.pgdg100+1
# Mon, 12 Jul 2021 22:25:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Mon, 12 Jul 2021 22:25:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 22:25:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 22:25:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 22:25:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 22:25:26 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 22:25:26 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Mon, 12 Jul 2021 22:25:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Jul 2021 22:25:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 22:25:27 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 22:25:27 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 22:25:28 GMT
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
	-	`sha256:add1501eead671e619dc4b891f20c1e9fb63acaff60c09a3664f7328327bba61`  
		Last Modified: Mon, 12 Jul 2021 22:32:16 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c99dd9800a53c3606a14191b5931e070bb2d9fd72d87bb80be11d28b706c4be`  
		Last Modified: Mon, 12 Jul 2021 22:35:30 GMT  
		Size: 40.7 MB (40749178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c64d2ec9a81a560eaa6230b98865ee50a102b2e7eea434c2017f2f07769c59e`  
		Last Modified: Mon, 12 Jul 2021 22:35:22 GMT  
		Size: 7.9 KB (7869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5118e37a9b0d1fe6555e650a60283237b2e1e3b4d528f473bb3f09bef154675f`  
		Last Modified: Mon, 12 Jul 2021 22:35:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fe6fb4de5fda084c1c0a03969f7cee3709b18cd871c66ae613b1e1b060b7e1`  
		Last Modified: Mon, 12 Jul 2021 22:35:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17054bfc614fb693f138d470a627819ef71c444db46df01361aa4df7248bfbd`  
		Last Modified: Mon, 12 Jul 2021 22:35:21 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cb105d9cfd3997765dee4cb18e7263b16ee213564afb614c4d21308273376d`  
		Last Modified: Mon, 12 Jul 2021 22:35:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-buster` - linux; arm variant v5

```console
$ docker pull postgres@sha256:35123af456576e4a1345cb42efd2aa83f706639b9a265620e372935d4853e2e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.6 MB (77606157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8630e42a8badd26b6f71725ef945153e6ae77b2f7e9ded064ab9d831164c5441`
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
# Wed, 23 Jun 2021 11:59:55 GMT
ENV PG_MAJOR=9.6
# Wed, 23 Jun 2021 11:59:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Wed, 23 Jun 2021 11:59:56 GMT
ENV PG_VERSION=9.6.22-1.pgdg100+1
# Wed, 23 Jun 2021 12:23:45 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 12:23:49 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 12:23:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 12:23:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 12:23:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 12:23:58 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 12:24:00 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Wed, 23 Jun 2021 12:24:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 12:24:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 12:24:05 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 12:24:05 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 12:24:07 GMT
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
	-	`sha256:4f874488d964779cf0ab8547717f33c2a64973b14cec65d83b75683289967820`  
		Last Modified: Wed, 23 Jun 2021 12:59:52 GMT  
		Size: 39.1 MB (39126961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51041e683c12a53b2c96ffde47cc5be6e43708f02ab8231dbabbd0bc4afeeb59`  
		Last Modified: Wed, 23 Jun 2021 12:59:21 GMT  
		Size: 7.9 KB (7873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df6a53f463b2cd65fac25f1a1b250b33b0eb0b5e81671bee9add398bd4eff6a`  
		Last Modified: Wed, 23 Jun 2021 12:59:21 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ddc40afddbf15119494140529c88bede9641dbe9d176ea1c73cd23b14d3998`  
		Last Modified: Wed, 23 Jun 2021 12:59:21 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b56cd122e32521e7aca034a82c5b21ef64e1333000ed88683a60ac697faf1c`  
		Last Modified: Wed, 23 Jun 2021 12:59:21 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbda0d9c3a216873088e53ede35453dc9814f65986784d0abafc5ec94c26603`  
		Last Modified: Wed, 23 Jun 2021 12:59:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-buster` - linux; arm variant v7

```console
$ docker pull postgres@sha256:3bbd3aa34cfd4a9651cec2bf20ac25cd00e209b9793f4d9d8129a08486a9ac99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.0 MB (74007447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5cac77364c9a6d0b953a3896516569e41afec5709281573eb02153bf8f02a66`
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
# Wed, 23 Jun 2021 21:59:24 GMT
ENV PG_MAJOR=9.6
# Wed, 23 Jun 2021 21:59:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Wed, 23 Jun 2021 21:59:25 GMT
ENV PG_VERSION=9.6.22-1.pgdg100+1
# Wed, 23 Jun 2021 22:20:35 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 22:20:37 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 22:20:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 22:20:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 22:20:40 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 22:20:41 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 22:20:41 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Wed, 23 Jun 2021 22:20:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 22:20:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 22:20:44 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 22:20:44 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 22:20:45 GMT
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
	-	`sha256:4c735eb5070067a35e1ac7a25daa9a4247fd2c5c5901d052dc3888518bd5e313`  
		Last Modified: Wed, 23 Jun 2021 22:55:11 GMT  
		Size: 38.0 MB (38041211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6af84cfcd439a37654bfaea7645f7f8b0d0cbaefcd43e865462c8366cbb4739`  
		Last Modified: Wed, 23 Jun 2021 22:54:42 GMT  
		Size: 7.9 KB (7872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834a9542a514058890381093886884d470cc0d1971987a672438320b7efd7cc3`  
		Last Modified: Wed, 23 Jun 2021 22:54:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321a6b547d8d8f2c78f6733bd499f2901eeecc4e0b2bd13979bba8599c91698e`  
		Last Modified: Wed, 23 Jun 2021 22:54:42 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099f9650f588d4b6e485d611a6f7c93eff778d757d04df0cda61a90fc852f6bd`  
		Last Modified: Wed, 23 Jun 2021 22:54:42 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9a4f6fd29717de480069d2023ed5bed1750cb38b7836698c3aa3adab72269e`  
		Last Modified: Wed, 23 Jun 2021 22:54:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-buster` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:e78857d676d6a8ba3108a587d7cad22cc0c87a4fcdd0c43088cda57aa31f61b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80274331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d034fe944c82cc7e0c2d6cf602d7c899f9887d6be5dcb671ababac3ed527b415`
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
# Mon, 12 Jul 2021 22:42:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Mon, 12 Jul 2021 23:03:43 GMT
ENV PG_MAJOR=9.6
# Mon, 12 Jul 2021 23:03:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Mon, 12 Jul 2021 23:03:43 GMT
ENV PG_VERSION=9.6.22-1.pgdg100+1
# Mon, 12 Jul 2021 23:03:59 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Mon, 12 Jul 2021 23:04:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 23:04:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 23:04:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 23:04:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 23:04:02 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 23:04:02 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Mon, 12 Jul 2021 23:04:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Jul 2021 23:04:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 23:04:04 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 23:04:04 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 23:04:04 GMT
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
	-	`sha256:411aeed71a6426703d10aea2cf14e0a4182facfd67088c46261de8c1cf38092b`  
		Last Modified: Mon, 12 Jul 2021 23:21:08 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63eb5e5899649e8286ec3f9b3a82b8fba44f8d67a8f3f731968e4e13ef244fb`  
		Last Modified: Mon, 12 Jul 2021 23:24:51 GMT  
		Size: 40.5 MB (40462424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e746935324e65118a000ced57faff36b131857b435592685f64a03bb1bb521`  
		Last Modified: Mon, 12 Jul 2021 23:24:41 GMT  
		Size: 7.9 KB (7871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4e7c745bc76f6af3d86da873975a785881b742227b46759dfa1b48edd65653`  
		Last Modified: Mon, 12 Jul 2021 23:24:41 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac396053d590ea230fd1086e86907bd20f63bdd27d9892fac8edd1a0eb24778`  
		Last Modified: Mon, 12 Jul 2021 23:24:42 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55207fabedf948be3faeefe20d26a52ed893fa519fa73fbac7a1923fae73a10d`  
		Last Modified: Mon, 12 Jul 2021 23:24:41 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7a70e940aabdef72d8998192284064c7a23ddbda762da1e7830532f80f826`  
		Last Modified: Mon, 12 Jul 2021 23:24:42 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-buster` - linux; 386

```console
$ docker pull postgres@sha256:c571b6c9c7c033c80fdcbf26548e41419b14595552cda9fd57b8e8b30a7a8ebd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83065446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d90fedd5d7465bb4db69260fb010da10accddb4c8726f8e3d8f659a89e7b60dd`
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
# Mon, 12 Jul 2021 22:40:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Mon, 12 Jul 2021 22:44:33 GMT
ENV PG_MAJOR=9.6
# Mon, 12 Jul 2021 22:44:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Mon, 12 Jul 2021 22:44:33 GMT
ENV PG_VERSION=9.6.22-1.pgdg100+1
# Mon, 12 Jul 2021 22:44:50 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Mon, 12 Jul 2021 22:44:52 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 22:44:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 22:44:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 22:44:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 22:44:54 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 22:44:54 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Mon, 12 Jul 2021 22:44:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Jul 2021 22:44:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 22:44:55 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 22:44:55 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 22:44:55 GMT
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
	-	`sha256:9b94e6fab5aba51a011ac98fce2529cb56892d5da34ee9d916fd8401dc059861`  
		Last Modified: Mon, 12 Jul 2021 22:53:59 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3453d6c4d3a185d1ec7137a8e63eccda61bed0560e2e626d2ed7f604c16f594`  
		Last Modified: Mon, 12 Jul 2021 22:57:58 GMT  
		Size: 41.0 MB (40953967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920e442b8f9a802961df2c05ab7cc973018015eacaea5b37817e9cb03520b26`  
		Last Modified: Mon, 12 Jul 2021 22:57:47 GMT  
		Size: 7.9 KB (7874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97a4c2fb4f25b908739cbbe20d7af335d3611291786a822c4e4a472e9a3c00a`  
		Last Modified: Mon, 12 Jul 2021 22:57:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709977cc579386a37d7f9f2c0913a2fa4c203b74833181333e001a19f9660a23`  
		Last Modified: Mon, 12 Jul 2021 22:57:47 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340ba78d3947f015f84dc790851241ee8ca552da63779e8d29f8cc86d85d9f93`  
		Last Modified: Mon, 12 Jul 2021 22:57:47 GMT  
		Size: 4.4 KB (4399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9b85b037185d28a93898264686eb8afc3b35852303a5a41ee06d6a25eb61a4`  
		Last Modified: Mon, 12 Jul 2021 22:57:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-buster` - linux; mips64le

```console
$ docker pull postgres@sha256:cf6d4bb690033f32c0469dfe4532451ba738b31f32b5e79aae5071d8420ad020
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.0 MB (79035845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd6a9e10fe34dfe1c8186df8191e22b5cd9113d853e0ad99aea78dce6c85f085`
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
# Wed, 23 Jun 2021 09:16:26 GMT
ENV PG_MAJOR=9.6
# Wed, 23 Jun 2021 09:16:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Wed, 23 Jun 2021 09:16:27 GMT
ENV PG_VERSION=9.6.22-1.pgdg100+1
# Wed, 23 Jun 2021 09:51:08 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 09:51:10 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 09:51:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 09:51:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 09:51:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 09:51:15 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 09:51:15 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Wed, 23 Jun 2021 09:51:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 09:51:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 09:51:18 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 09:51:18 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 09:51:19 GMT
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
	-	`sha256:a5bc0556b941af91a4da527c3c179c06bfc0d74c8897feff1d77fa8a946a6941`  
		Last Modified: Wed, 23 Jun 2021 09:56:33 GMT  
		Size: 39.4 MB (39361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c186b2c5154405dd3b0f4baf157070a6dbb6c29d489bf897afbae3872947aef3`  
		Last Modified: Wed, 23 Jun 2021 09:56:01 GMT  
		Size: 7.9 KB (7876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba56682c5d174b5dd1a223a983a5ff92e19568162c6ae477159729b7a9ff293`  
		Last Modified: Wed, 23 Jun 2021 09:56:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd37dbcedd0a440350a1c899e27822b975ef03c64cb32a57164b27b5a56b9b35`  
		Last Modified: Wed, 23 Jun 2021 09:56:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43eb1f177754d713cf4a718b65f903272077e0a569d83efa8d7904ae45ea97f`  
		Last Modified: Wed, 23 Jun 2021 09:56:01 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cf42f6fcc8a94a6e4bf2e696ccbb682a6db71df6f527e3ca5931fa9f21a25e`  
		Last Modified: Wed, 23 Jun 2021 09:56:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-buster` - linux; ppc64le

```console
$ docker pull postgres@sha256:6f307af71e32ee692bd945e886720010faa509cc8919388a49217c4346ff7a51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87894617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02724fd42e3ff3d057f87b690c3631a2f0b8eb01dc87da7173a151259ead169c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 09:26:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Jul 2021 09:27:08 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 10 Jul 2021 09:27:11 GMT
ENV GOSU_VERSION=1.12
# Sat, 10 Jul 2021 09:28:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 10 Jul 2021 09:28:50 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 10 Jul 2021 09:28:54 GMT
ENV LANG=en_US.utf8
# Sat, 10 Jul 2021 09:29:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 09:29:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 12 Jul 2021 22:25:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Mon, 12 Jul 2021 22:51:20 GMT
ENV PG_MAJOR=9.6
# Mon, 12 Jul 2021 22:51:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Mon, 12 Jul 2021 22:51:35 GMT
ENV PG_VERSION=9.6.22-1.pgdg100+1
# Mon, 12 Jul 2021 22:53:34 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Mon, 12 Jul 2021 22:53:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 22:54:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 22:54:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 22:54:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 22:54:43 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 22:54:49 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Mon, 12 Jul 2021 22:55:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Jul 2021 22:55:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 22:55:11 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 22:55:15 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 22:55:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f44e1b7ec359574101b6423ee542a7080fc19feca9eff255c2958a11e68b7c`  
		Last Modified: Sat, 10 Jul 2021 10:08:29 GMT  
		Size: 5.0 MB (4967521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f9abdef7b99668fc38830311d51f8f88c61beae6f1f9f34f2c040ca74b192d`  
		Last Modified: Sat, 10 Jul 2021 10:08:27 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb4a9ccef3e18f2aed3290895872d80dc858724af563c30bfc57b8f6b78eb4`  
		Last Modified: Sat, 10 Jul 2021 10:08:26 GMT  
		Size: 1.3 MB (1338188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74741ade7f637585371fb269094dbe53dbf8123e179c12fcd0ef0f8b51ae1394`  
		Last Modified: Sat, 10 Jul 2021 10:08:26 GMT  
		Size: 8.0 MB (7965490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220a1a7e817c30d268e11c2bb6648eb543cfbcff66ce7578b4c7d0f09f811ef`  
		Last Modified: Sat, 10 Jul 2021 10:08:25 GMT  
		Size: 397.1 KB (397090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68dc5c77671536375c3c90a625b608ce8515793bab6c81f7c6f3e7061ae0650`  
		Last Modified: Sat, 10 Jul 2021 10:08:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46de291ff3594e1dd9e8d64a23509549e8d7d16d914511afe8eb8a4203a63857`  
		Last Modified: Mon, 12 Jul 2021 23:29:37 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025dd555d5a5cd25b327950d42fd5da7959c8b2dd4a19bca1e1d463da74e9c1d`  
		Last Modified: Mon, 12 Jul 2021 23:32:09 GMT  
		Size: 42.7 MB (42654951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf15ce8ccc966173b65adc3d706ff125bb5b529a0ce1962a9065c2e2d079748`  
		Last Modified: Mon, 12 Jul 2021 23:31:57 GMT  
		Size: 7.9 KB (7879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c516ff10d59d9cad13f5e2c7cc93d73321043749d929887e6ede01b5f381a7`  
		Last Modified: Mon, 12 Jul 2021 23:31:57 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9be475e425ad1f7f780cbb1b48e88d1195112460f772d4442f51bac6825d179`  
		Last Modified: Mon, 12 Jul 2021 23:31:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c3f28a91009b66b4a929b3df5c43bc39a66b6ef4e3511f0adfcd3b9ab4d89b`  
		Last Modified: Mon, 12 Jul 2021 23:31:57 GMT  
		Size: 4.4 KB (4404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4540b0bbc8a531f4f51b63a8e732aab2775277fe2c9b525164b184929335c6e`  
		Last Modified: Mon, 12 Jul 2021 23:31:57 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-buster` - linux; s390x

```console
$ docker pull postgres@sha256:a5837783f11903417bc82bfb7bc85cc7781f31d9d1353573af9ef5836bc540a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.3 MB (80297770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe58f329aa2136aa249271e9c8366092bdfd7874a1b27b3e6bc1aba81d043755`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 08:50:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 09 Jul 2021 08:50:08 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 09 Jul 2021 08:50:08 GMT
ENV GOSU_VERSION=1.12
# Fri, 09 Jul 2021 08:50:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 09 Jul 2021 08:50:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 09 Jul 2021 08:50:55 GMT
ENV LANG=en_US.utf8
# Fri, 09 Jul 2021 08:51:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 08:51:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 12 Jul 2021 22:48:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Mon, 12 Jul 2021 23:52:47 GMT
ENV PG_MAJOR=9.6
# Mon, 12 Jul 2021 23:52:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Mon, 12 Jul 2021 23:52:48 GMT
ENV PG_VERSION=9.6.22-1.pgdg100+1
# Tue, 13 Jul 2021 00:07:44 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 13 Jul 2021 00:07:50 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Jul 2021 00:07:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Jul 2021 00:07:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Jul 2021 00:07:55 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Jul 2021 00:07:56 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Jul 2021 00:07:57 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Tue, 13 Jul 2021 00:07:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Jul 2021 00:08:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jul 2021 00:08:00 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jul 2021 00:08:01 GMT
EXPOSE 5432
# Tue, 13 Jul 2021 00:08:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e24c9c5b765282dc5e079bdeac6f3999a97724c44adc0c8d6108a5ed55990c`  
		Last Modified: Fri, 09 Jul 2021 10:19:30 GMT  
		Size: 4.1 MB (4060319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70cb54829bcf48c25c86f7fefb6f44b0b607dd4e8f4ee700f8fde682d2ec93af`  
		Last Modified: Fri, 09 Jul 2021 10:19:29 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f7828c959776b26a1ff7f70840f99877a4332769f49985224d911d631fad93`  
		Last Modified: Fri, 09 Jul 2021 10:19:29 GMT  
		Size: 1.4 MB (1406333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c230ee76583ca1aaf2db3201f68e3a02bffbcfb842940cf8d0426e1eda438a`  
		Last Modified: Fri, 09 Jul 2021 10:19:29 GMT  
		Size: 8.0 MB (8019586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3707e28fc50cac335aa091fdcbe9e346800918f56b58adaf45b415c55b7ce8a`  
		Last Modified: Fri, 09 Jul 2021 10:19:27 GMT  
		Size: 388.5 KB (388506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6321ccfb103040358d4e043f3ca7de3b369069582fa1e1c8ce61dba5eea9357f`  
		Last Modified: Fri, 09 Jul 2021 10:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac68045d01301629acec617ba467ad2d7714fe189072a7123a27e179de90ae8`  
		Last Modified: Tue, 13 Jul 2021 00:44:51 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3e025e22c2ec07642149e5c4776cc50cd0807cfb75702d0615d45d43e28fa0`  
		Last Modified: Tue, 13 Jul 2021 00:46:27 GMT  
		Size: 40.6 MB (40644565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89736dd1a8bd24dcdb6969ee855dda49b10d84644a5b23c40768954c466304ca`  
		Last Modified: Tue, 13 Jul 2021 00:46:19 GMT  
		Size: 7.9 KB (7878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61810b266fa3fd5b87b6f6ba109c732537f1726d7269ade648525b3eb774dfee`  
		Last Modified: Tue, 13 Jul 2021 00:46:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665d39e55a59b04fda8047488fec8e5c2a8f38cee9dada3b3fc0386c53dce8a0`  
		Last Modified: Tue, 13 Jul 2021 00:46:19 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208fda6f4ac967edb4f9cdb8cbe06182776896f35eb2c066ad5d3c816f95e692`  
		Last Modified: Tue, 13 Jul 2021 00:46:19 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6a4748b905ca601572a1b2f6b079d9d9c091442852a399c414139e9eb68b51`  
		Last Modified: Tue, 13 Jul 2021 00:46:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
