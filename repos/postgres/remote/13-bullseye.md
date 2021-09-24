## `postgres:13-bullseye`

```console
$ docker pull postgres@sha256:5bf3a049b6f119acbe192b82aadd801e82cd641f94ab529230bac050cebc95e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `postgres:13-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:b3afa7d78b17d1ceb13e8727c25d953a7ad149fbd5de2b9050fe2fb3983c7219
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135748675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5861c038d674e4db6377d9f3880e66e028d276c9a32c9688fb1afd9b497ba78b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:21 GMT
ADD file:19d7ba0fceddd7fc78b5fb96cf8110e5d10e0e5d2554030dfe640d161379cb79 in / 
# Fri, 03 Sep 2021 01:21:21 GMT
CMD ["bash"]
# Thu, 23 Sep 2021 23:48:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Sep 2021 23:48:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Sep 2021 23:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Sep 2021 23:48:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Sep 2021 23:48:51 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Sep 2021 23:48:51 GMT
ENV LANG=en_US.utf8
# Thu, 23 Sep 2021 23:48:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Sep 2021 23:48:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Sep 2021 23:49:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 23 Sep 2021 23:56:06 GMT
ENV PG_MAJOR=13
# Thu, 23 Sep 2021 23:56:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Thu, 23 Sep 2021 23:56:07 GMT
ENV PG_VERSION=13.4-1.pgdg110+1
# Thu, 23 Sep 2021 23:56:29 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Sep 2021 23:56:30 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 23:56:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 23:56:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 23:56:32 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 23:56:32 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 23:56:33 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Thu, 23 Sep 2021 23:56:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 23:56:33 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 23:56:33 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 23:56:34 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f8416d8bac72cefc0ce17bd2dc0c03aa43e123d309db92ee23be9382192cf2ed`  
		Last Modified: Fri, 03 Sep 2021 01:27:25 GMT  
		Size: 31.4 MB (31368702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858331474a6973db99f1d2343adebce057c67fa5a394c38cb84d7e38310198fe`  
		Last Modified: Fri, 24 Sep 2021 00:00:17 GMT  
		Size: 4.4 MB (4414347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee930e806cf68d514327ca629b1450ae5da5a5d4f75127380e21033b2a8e2ae`  
		Last Modified: Fri, 24 Sep 2021 00:00:14 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6748b551eaabf3a6f6a033cbd73645d6fee7756867336986c621ce6cb8beca3b`  
		Last Modified: Fri, 24 Sep 2021 00:00:14 GMT  
		Size: 1.5 MB (1450472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3885f0ed3c9aa6d6399bcb4953cbfe6380960ed6bc601d4ad1bcbebf4c9ba84a`  
		Last Modified: Fri, 24 Sep 2021 00:00:14 GMT  
		Size: 8.0 MB (8045261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aac1b6637a0995cfc53a2d2fe9487da28d86fe2aad5967f93e99506384e4ee`  
		Last Modified: Fri, 24 Sep 2021 00:00:13 GMT  
		Size: 441.5 KB (441491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67f57ae254c0d300e13c307ca8229df6cbbef6c1e677eb3b008215374a78eaf`  
		Last Modified: Fri, 24 Sep 2021 00:00:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cba9dccd3375aacc8b39f5bbb0a0366011d6b1cb52b44a419ebd75ea669e748`  
		Last Modified: Fri, 24 Sep 2021 00:00:11 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3eecc077fb516e01d1f2ab7e9d1703f3a3bc5247ddf123818f1c09e370f933`  
		Last Modified: Fri, 24 Sep 2021 00:01:08 GMT  
		Size: 90.0 MB (90009314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d31d2dbf986338f6c158ef537f1bb87361a8b91a21a092454e83bde57475d5`  
		Last Modified: Fri, 24 Sep 2021 00:00:54 GMT  
		Size: 9.4 KB (9352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c407080f1477be10ecab4b9258d86c1989b8a3a1443cc55e303d0ff93d9dd86f`  
		Last Modified: Fri, 24 Sep 2021 00:00:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57838d6b9005e55027da18edbe24c468359f5f649578c13afce16e3c3cc075a9`  
		Last Modified: Fri, 24 Sep 2021 00:00:54 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c5605263759bcdec35fa2ba5f3c45abdf2dda42ff18410fa9f1ee3ffffd17d`  
		Last Modified: Fri, 24 Sep 2021 00:00:54 GMT  
		Size: 4.4 KB (4400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:4cb113ae771ffab8a869246f90a2b5f031350f6b573c74b49dba177568c661a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128987367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f400d1b26f726cf27c89fb8a71b6baf6cf86731fad9a0f07e01ba27c70d5c59c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 00:50:28 GMT
ADD file:3370827f2aa0dc43cfc2dcb693f82d3f450a70850de7e2514117e366f660d302 in / 
# Fri, 03 Sep 2021 00:50:29 GMT
CMD ["bash"]
# Fri, 24 Sep 2021 03:02:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Sep 2021 03:02:38 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 24 Sep 2021 03:02:38 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Sep 2021 03:03:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Sep 2021 03:03:23 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 24 Sep 2021 03:03:24 GMT
ENV LANG=en_US.utf8
# Fri, 24 Sep 2021 03:03:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Sep 2021 03:03:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Sep 2021 03:03:47 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Fri, 24 Sep 2021 03:42:07 GMT
ENV PG_MAJOR=13
# Fri, 24 Sep 2021 03:42:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 24 Sep 2021 03:42:07 GMT
ENV PG_VERSION=13.4-1.pgdg110+1
# Fri, 24 Sep 2021 04:17:51 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 04:17:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 04:17:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 04:17:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 04:17:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 04:17:57 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 04:17:58 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 24 Sep 2021 04:17:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 04:17:59 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 04:17:59 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 04:17:59 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f97b1d091d60e08b0ff779d3cf24a016e55312c03d0930408ff1e1f18d486139`  
		Last Modified: Fri, 03 Sep 2021 01:05:38 GMT  
		Size: 28.9 MB (28910713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41158181d787a7d01ecd8b9addc68523e878a0b6822d38407b80580aead38eb1`  
		Last Modified: Fri, 24 Sep 2021 06:16:18 GMT  
		Size: 4.1 MB (4096378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3d1c9843729ef2d4e0a806843ef76f148f08da41cbf119d3c1e4317300c930`  
		Last Modified: Fri, 24 Sep 2021 06:16:15 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ad7444d4090e3e2907ad8f52043daceda04c84925bb9908441f754ec088a80`  
		Last Modified: Fri, 24 Sep 2021 06:16:15 GMT  
		Size: 1.4 MB (1409797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316e2189fd7c6de3363cf9650ad407059a32b1abb66630bf60cfc5fc329e1ee9`  
		Last Modified: Fri, 24 Sep 2021 06:16:19 GMT  
		Size: 8.0 MB (8045217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d43e915079df0ebb11eb71b6720d64278f2a762307e26c52b87661785a8e21`  
		Last Modified: Fri, 24 Sep 2021 06:16:14 GMT  
		Size: 439.8 KB (439809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e958fb6c5a837ba2e52e9aaa2c5244d3090b5145dd6bd831bb90855b786b8aab`  
		Last Modified: Fri, 24 Sep 2021 06:16:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e023ef71713d4b6b12271b3b6c9bfbe242193074a30e7b8bd2571a922828f32b`  
		Last Modified: Fri, 24 Sep 2021 06:16:13 GMT  
		Size: 3.1 KB (3052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2a2b8b592518530ce3dc09946a8027b55fda0b5d7db63884512684ab09b711`  
		Last Modified: Fri, 24 Sep 2021 06:18:12 GMT  
		Size: 86.1 MB (86066365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b11751f399c81dba7aca5c64c84eb267396ecb9081accd09093d6c3793ab8cc`  
		Last Modified: Fri, 24 Sep 2021 06:17:18 GMT  
		Size: 9.4 KB (9359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d479cd2c0ec7924c25812c8471186f4764981e6ca681e0a1d15b6c23fe959d`  
		Last Modified: Fri, 24 Sep 2021 06:17:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2e8754f9a7ff75a7955ee21035a12b31a2a578e87f365957f5b870ccedab41`  
		Last Modified: Fri, 24 Sep 2021 06:17:19 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774eae1aa7c5380d9de9b535033d9b040fa9325e127c8c4b38af8b633d34c995`  
		Last Modified: Fri, 24 Sep 2021 06:17:19 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:f1605a6736205177280d45b660e902acdc72bd66d9f407fed6470519f847b666
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130873549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:588250b21688859fbbd023b2426d590d5348514600be74f7b5377c53abc7251b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:33 GMT
ADD file:9600a4686ae105acffa54787a7c81f5252e90023cbcfbe37519150b954110c5c in / 
# Fri, 03 Sep 2021 00:40:34 GMT
CMD ["bash"]
# Fri, 24 Sep 2021 01:21:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Sep 2021 01:21:49 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 24 Sep 2021 01:21:49 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Sep 2021 01:21:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Sep 2021 01:22:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 24 Sep 2021 01:22:04 GMT
ENV LANG=en_US.utf8
# Fri, 24 Sep 2021 01:22:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Sep 2021 01:22:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Sep 2021 01:22:18 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Fri, 24 Sep 2021 01:27:38 GMT
ENV PG_MAJOR=13
# Fri, 24 Sep 2021 01:27:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 24 Sep 2021 01:27:39 GMT
ENV PG_VERSION=13.4-1.pgdg110+1
# Fri, 24 Sep 2021 01:27:57 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 01:27:58 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 01:27:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 01:27:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 01:28:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 01:28:00 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 01:28:00 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 24 Sep 2021 01:28:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 01:28:01 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 01:28:01 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 01:28:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1901ca797b5ea06f6a4facc81ad772177fdd833ed4329dc86ef126078633b949`  
		Last Modified: Fri, 03 Sep 2021 00:48:51 GMT  
		Size: 30.1 MB (30055483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d52aa16d23d6741fd9e6026a726d50f15f81ecc5c746bcfd45706b35e5669a`  
		Last Modified: Fri, 24 Sep 2021 01:32:42 GMT  
		Size: 4.4 MB (4415371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6d76f4cd6fd01d972121dff0e017af3ebbff49562c142463f2b05c84d32d28`  
		Last Modified: Fri, 24 Sep 2021 01:32:41 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932ea055db01e1e86f54eaf2aa12bbfa47be575402ce158382016b815942bf11`  
		Last Modified: Fri, 24 Sep 2021 01:32:41 GMT  
		Size: 1.4 MB (1386575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9845a88ef044fffc934cc31db52177750e1b9ed0abb7667067def9fa3ad37c`  
		Last Modified: Fri, 24 Sep 2021 01:32:40 GMT  
		Size: 8.0 MB (8045109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ba726c5e4bec74d8b625f74a8f66c62eb7c2dd8a56eea998ffcce028f47933`  
		Last Modified: Fri, 24 Sep 2021 01:32:39 GMT  
		Size: 442.0 KB (441996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a08bbd52cf66362b834c9f27bd70b0723029b09d605e0af6ba6f8099d58bb4`  
		Last Modified: Fri, 24 Sep 2021 01:32:39 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146eb9063918d472bdf2fb6cc814a21ed846a107117a8f2ebb0423d6deab8913`  
		Last Modified: Fri, 24 Sep 2021 01:32:38 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195670bb7915b0dba628900892ddcf1a0399abc380d5860c8e090406f60c041`  
		Last Modified: Fri, 24 Sep 2021 01:33:36 GMT  
		Size: 86.5 MB (86509927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edca1bf8dbf75b4945b22f7f679331ee901d1fd33b8bebef4f518c60d71ff4b`  
		Last Modified: Fri, 24 Sep 2021 01:33:23 GMT  
		Size: 9.4 KB (9353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18de8ccee9f3310065954412a6ab9b3b145112e641464840325c71b0ca208d47`  
		Last Modified: Fri, 24 Sep 2021 01:33:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a351759e28382e47e86a8d38b7a90bf87323c5b3e81f1f61b5fd6df3c5af2646`  
		Last Modified: Fri, 24 Sep 2021 01:33:23 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8c91fecf8eff04160267b70556fc8feeeca70630c9d540dc673df44ab8a4c8`  
		Last Modified: Fri, 24 Sep 2021 01:33:23 GMT  
		Size: 4.4 KB (4399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:f1ba92e1d7b820567cfa4385c573fcd4329515e1d55fc723353b23eb67f6953c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137834908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41dfcc84159972bc807169c6c98a8448ed3d88816a04a263b21edf9a5e42d2c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 00:39:52 GMT
ADD file:dcef0e50863a79295fdbbdad2086d337d6935a220550cb8adaedd7929bd7de63 in / 
# Fri, 03 Sep 2021 00:39:52 GMT
CMD ["bash"]
# Thu, 23 Sep 2021 22:56:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Sep 2021 22:56:35 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Sep 2021 22:56:36 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Sep 2021 22:56:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Sep 2021 22:56:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Sep 2021 22:56:54 GMT
ENV LANG=en_US.utf8
# Thu, 23 Sep 2021 22:56:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Sep 2021 22:57:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Sep 2021 22:57:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 23 Sep 2021 23:19:42 GMT
ENV PG_MAJOR=13
# Thu, 23 Sep 2021 23:19:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Thu, 23 Sep 2021 23:19:42 GMT
ENV PG_VERSION=13.4-1.pgdg110+1
# Thu, 23 Sep 2021 23:34:02 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Sep 2021 23:34:03 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 23:34:04 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 23:34:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 23:34:05 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 23:34:06 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 23:34:06 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Thu, 23 Sep 2021 23:34:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 23:34:06 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 23:34:07 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 23:34:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e16e03ac165c3106d1f4265c32840999585f4c4f0e56bd13286caeef08c5be9a`  
		Last Modified: Fri, 03 Sep 2021 00:48:04 GMT  
		Size: 32.4 MB (32379875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f5c729250790434f2cf02b08fd37659230bf2003cbb8dda15b2b439925b5b7`  
		Last Modified: Fri, 24 Sep 2021 00:32:34 GMT  
		Size: 4.8 MB (4812799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01b4bf984014c2656db1ac585cf5b5e68cc0649e13732d5f513d5584574fb24`  
		Last Modified: Fri, 24 Sep 2021 00:32:30 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4fc5db44e4a6721664ec1bfbf83cad44ecc6473df997770db9991a33375542`  
		Last Modified: Fri, 24 Sep 2021 00:32:31 GMT  
		Size: 1.4 MB (1420892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159b11f2bcfcc3d6de7baa7eca393a1668e01c4c7ec4a7a8beb6535f8c89de9a`  
		Last Modified: Fri, 24 Sep 2021 00:32:33 GMT  
		Size: 8.0 MB (8045095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea6fdd893403f75e180ca8983457e3ae9b291ee2752e52f20ba755484e31d44`  
		Last Modified: Fri, 24 Sep 2021 00:32:28 GMT  
		Size: 447.9 KB (447894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87644a6d8d9ea385ca4e078446b394079e14023a798d2a1f88efe0a219c581a`  
		Last Modified: Fri, 24 Sep 2021 00:32:28 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4115a3c8ed9471f6daf778fd45556f9f39484db13d213945921b157a6983ae0d`  
		Last Modified: Fri, 24 Sep 2021 00:32:28 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f957748e4df36e6839ff0ce4162e813e7eb0561a5f767ebc5b4b392b8e211c`  
		Last Modified: Fri, 24 Sep 2021 00:34:14 GMT  
		Size: 90.7 MB (90709260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56af3fd6ff9408b738325a046c1d25eec2a61dcfcfa13dd1aabe511f0b5a28a`  
		Last Modified: Fri, 24 Sep 2021 00:33:47 GMT  
		Size: 9.4 KB (9357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a4d028a6d74f670920d034e685d8c10593e2d49240cd3d0c3b2e17083857ca`  
		Last Modified: Fri, 24 Sep 2021 00:33:47 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6edc82e018828f32d95e61b80b3cce08cbceb145f98593bed4dc43e4e3edb34`  
		Last Modified: Fri, 24 Sep 2021 00:33:47 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbd98389143204a53b58eae2ea5390d6723b5c2d1c7625a9b3697b964078643`  
		Last Modified: Fri, 24 Sep 2021 00:33:47 GMT  
		Size: 4.4 KB (4409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:65acd906385ac3cf03f990e48291271b06d0f880d6c6288dd9de77876ff744f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130561568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed79eb20ad275f7d6cc88be5e16a7010bc048ab545b9ddc46b42f8c800ce1757`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 01:10:01 GMT
ADD file:e842559443fb9351f1a9ac9ce03dfe0b069d8b9c3409f8d9b21abcbdc2a437c5 in / 
# Fri, 03 Sep 2021 01:10:02 GMT
CMD ["bash"]
# Thu, 23 Sep 2021 22:49:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Sep 2021 22:49:26 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Sep 2021 22:49:27 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Sep 2021 22:49:47 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Sep 2021 22:50:11 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Sep 2021 22:50:12 GMT
ENV LANG=en_US.utf8
# Thu, 23 Sep 2021 22:50:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Sep 2021 22:50:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Sep 2021 22:50:29 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 23 Sep 2021 23:46:53 GMT
ENV PG_MAJOR=13
# Thu, 23 Sep 2021 23:46:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Thu, 23 Sep 2021 23:46:54 GMT
ENV PG_VERSION=13.4-1.pgdg110+1
# Fri, 24 Sep 2021 00:39:43 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 00:39:46 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 00:39:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 00:39:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 00:39:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 00:39:51 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 00:39:51 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 24 Sep 2021 00:39:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 00:39:52 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 00:39:52 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 00:39:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2320664dc3760d5d905a15eef2bf52da0cbab097fb4fc626c1f96722a2e2188c`  
		Last Modified: Fri, 03 Sep 2021 01:18:25 GMT  
		Size: 29.6 MB (29627416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0e4f59ff7aec890c8d9a5345824960f761b0466c7ff3461557a84100f7748e`  
		Last Modified: Fri, 24 Sep 2021 03:31:48 GMT  
		Size: 4.4 MB (4402755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b63c840cfd6434e8f77fcb81da66991d59a59229e576be90298d4a284a191a`  
		Last Modified: Fri, 24 Sep 2021 03:31:44 GMT  
		Size: 1.8 KB (1771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62a303182a41599697b70fe0efad146882b5d00dc21fdd86373da4552c06eee`  
		Last Modified: Fri, 24 Sep 2021 03:31:46 GMT  
		Size: 1.3 MB (1339274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2ebe66e561365127c39cc7f47473cac916e70361f452932c1256c1274e49ce`  
		Last Modified: Fri, 24 Sep 2021 03:31:49 GMT  
		Size: 8.0 MB (8044039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee3adb2f8367a039254f0a494ce6d4db17930a15c941711485d0303b3f3f058`  
		Last Modified: Fri, 24 Sep 2021 03:31:41 GMT  
		Size: 439.1 KB (439141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cac1a4c3c91d0c7b2f53df71d0aa35a7135108ac9c4488ada081117609f3d4`  
		Last Modified: Fri, 24 Sep 2021 03:31:42 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e1798d74c13e743a6547f8f83f4d0e042f5178d9cf70866bf9494facddae61`  
		Last Modified: Fri, 24 Sep 2021 03:31:41 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb271be3f6ba9fa21d85a3ae5d4c76019513abf1a3034652f874c0e98d8170`  
		Last Modified: Fri, 24 Sep 2021 03:33:52 GMT  
		Size: 86.7 MB (86689943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7a8b2c4327f67fa94bef999a374871dc3c0d7b2a27f5eaf8fea19368194754`  
		Last Modified: Fri, 24 Sep 2021 03:32:52 GMT  
		Size: 9.4 KB (9362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c370e9e6543aed8325269a3059d3e839237874df5e4de1abcb561dc06ba72bca`  
		Last Modified: Fri, 24 Sep 2021 03:32:52 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2e226cd2f38aea8067147337f4b16243303388df43567052e966a8735a13b6`  
		Last Modified: Fri, 24 Sep 2021 03:32:52 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a3faf4647dcf169ef48d793e5722794ccd2c3badf1a66413a830cfa8255bed`  
		Last Modified: Fri, 24 Sep 2021 03:32:52 GMT  
		Size: 4.4 KB (4399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:cd0fe8604a88aee97cc121015958f22452bb5069b79866c7c9efcc7d90048c21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144586921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dc769fe6e14dce15ea19676083b5813d6f845c114c888130eefb6a4dd759a37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:11 GMT
ADD file:71b4f3130e43c12907b826b33d9869308eec40607243a12d904fe47311431db9 in / 
# Fri, 03 Sep 2021 01:23:21 GMT
CMD ["bash"]
# Fri, 24 Sep 2021 06:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Sep 2021 06:41:05 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 24 Sep 2021 06:41:09 GMT
ENV GOSU_VERSION=1.12
# Fri, 24 Sep 2021 06:41:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Sep 2021 06:42:24 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 24 Sep 2021 06:42:28 GMT
ENV LANG=en_US.utf8
# Fri, 24 Sep 2021 06:42:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Sep 2021 06:42:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Sep 2021 06:43:23 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Fri, 24 Sep 2021 06:54:37 GMT
ENV PG_MAJOR=13
# Fri, 24 Sep 2021 06:54:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 24 Sep 2021 06:55:04 GMT
ENV PG_VERSION=13.4-1.pgdg110+1
# Fri, 24 Sep 2021 06:57:49 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 06:58:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 06:58:39 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 06:58:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 06:59:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 06:59:04 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 06:59:08 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 24 Sep 2021 06:59:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 06:59:26 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 06:59:38 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 06:59:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:be889fbf38c25cf263aa8d8c960d58470da7f841ab3f4949b8a1ac5c4514956c`  
		Last Modified: Fri, 03 Sep 2021 01:36:58 GMT  
		Size: 35.3 MB (35272405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78451690111a913c5499a9ff7786d97590a9203ac1a04bb6fe2fa324206f1b3`  
		Last Modified: Fri, 24 Sep 2021 07:19:35 GMT  
		Size: 5.2 MB (5222898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a735c32a8a0427c9cb951efcdfbd6adf2d9c8527e97f69f799d8b0d3ba64e`  
		Last Modified: Fri, 24 Sep 2021 07:19:30 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc7bf5779ae396f9fad96bd00ed6ee1674203342cc5300b7da52ff9bdc7aba9`  
		Last Modified: Fri, 24 Sep 2021 07:19:29 GMT  
		Size: 1.4 MB (1369922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c59d4db9df2958ed746d5a937b6f2497dfd27036b275de0f765f16bfb990025`  
		Last Modified: Fri, 24 Sep 2021 07:19:30 GMT  
		Size: 8.0 MB (8045375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdc8fb5c8e5f9e2865f8eb092e5b91801e89d9362da06a959feb61e81fee2a6`  
		Last Modified: Fri, 24 Sep 2021 07:19:29 GMT  
		Size: 451.5 KB (451530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53903b1e6ec7f7a7a42661fd450c56ef8514337a73726f43bad51777808d3717`  
		Last Modified: Fri, 24 Sep 2021 07:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d0e5b7dc9ef3e07bad0618096c70ff27bdc5befd7bf42ecf52cd5c6eb90349`  
		Last Modified: Fri, 24 Sep 2021 07:19:26 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb592ebbf86388546f4b0e8430d88dfb7a578b0a8b15fbabc7717a24f2ad5b81`  
		Last Modified: Fri, 24 Sep 2021 07:20:34 GMT  
		Size: 94.2 MB (94205678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6caeacf956a7242639dbbba4b2ced21e94dc86e28413de033bb5db3d1d8885ea`  
		Last Modified: Fri, 24 Sep 2021 07:20:17 GMT  
		Size: 9.4 KB (9364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95d92ac491ab191c95c21477d7845a6f557be8efea9e8ce1a4689f9bee503ef`  
		Last Modified: Fri, 24 Sep 2021 07:20:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29ef13304b5de4e84635f5945420e57493b42bf2fffd76205f529976456390b`  
		Last Modified: Fri, 24 Sep 2021 07:20:17 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccec18cace4fca6ca94f8253f7e19080ec334e443e748408842cebc2b5c865b`  
		Last Modified: Fri, 24 Sep 2021 07:20:17 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:5f605f1fa9def8505acf23622f9a062fbe78a42e998f5542cf4a222b77e47ec6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139490707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e107c0e3eed48978b0f8fed12132cc5ca0c7671043f4b2fa86cfcf8f5f719a4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 00:43:48 GMT
ADD file:9e72d98b2c920e433c6b776ed8eaf6a90cbf367d0ee37a8461d191499be72d39 in / 
# Fri, 03 Sep 2021 00:43:52 GMT
CMD ["bash"]
# Thu, 23 Sep 2021 22:40:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Sep 2021 22:40:36 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Sep 2021 22:40:36 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Sep 2021 22:40:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Sep 2021 22:40:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Sep 2021 22:40:50 GMT
ENV LANG=en_US.utf8
# Thu, 23 Sep 2021 22:40:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Sep 2021 22:40:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Sep 2021 22:41:00 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 23 Sep 2021 22:54:03 GMT
ENV PG_MAJOR=13
# Thu, 23 Sep 2021 22:54:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Thu, 23 Sep 2021 22:54:03 GMT
ENV PG_VERSION=13.4-1.pgdg110+1
# Thu, 23 Sep 2021 23:03:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Sep 2021 23:03:26 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 23:03:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 23:03:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 23:03:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 23:03:27 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 23:03:28 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Thu, 23 Sep 2021 23:03:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 23:03:28 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 23:03:28 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 23:03:29 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:33fe066e16e87fca4bcb280b7ec53d44c561299928e592068e985314cf93215b`  
		Last Modified: Fri, 03 Sep 2021 00:52:58 GMT  
		Size: 29.7 MB (29650625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9574a728e4abef27edb93d7aeef4bf9573bf611327b83bb5b9ae0cf3b51a01aa`  
		Last Modified: Thu, 23 Sep 2021 23:35:08 GMT  
		Size: 4.3 MB (4302140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13962b60bfa73a6792b7b2e5fac03a640b92942196e5d72a0833d8e3a7acfb7`  
		Last Modified: Thu, 23 Sep 2021 23:35:07 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85b52edea2e740a86a92748e288257764cd6aec018010800053a3b064a1ea8a`  
		Last Modified: Thu, 23 Sep 2021 23:35:07 GMT  
		Size: 1.4 MB (1437289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fbeac21b86966d815fda37a4a38a39a6f0eb020887d9798ef884cde53021e4`  
		Last Modified: Thu, 23 Sep 2021 23:35:07 GMT  
		Size: 8.1 MB (8098996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5ae0ca9f2feb3393203089d1ed95c97c0f35cfb0abcc59dab9aa92287a9c28`  
		Last Modified: Thu, 23 Sep 2021 23:35:06 GMT  
		Size: 438.2 KB (438231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71274debec8c352288e89548cb941c2dc41ca62e3ff205fb43f6f6eb15d85f2c`  
		Last Modified: Thu, 23 Sep 2021 23:35:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4838e35a4762b8143094b620112518a53d9c51723847b1e3ce6c2f13440c3bad`  
		Last Modified: Thu, 23 Sep 2021 23:35:06 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c170584de1bd00ad5d592ce06d6052f0fe6cc2c012b203fee350ab8ff3d5401b`  
		Last Modified: Thu, 23 Sep 2021 23:35:50 GMT  
		Size: 95.5 MB (95544325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee2f4ab8ca40edbcfa04866607c0201ce1f3e64b2bd0c225225811d9f60e821`  
		Last Modified: Thu, 23 Sep 2021 23:35:38 GMT  
		Size: 9.4 KB (9357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b196e86a31bfac96cd9475f2cc323991a00023a6ba17eba2bab5fff0af9ab3`  
		Last Modified: Thu, 23 Sep 2021 23:35:38 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dad683d18ba5dd949d22b73ab38a921383993301d78d858d253800d8cb29a4f`  
		Last Modified: Thu, 23 Sep 2021 23:35:38 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2063dc39555d30d6efa6c4b882ee19a2127af46e31ac505851bddde1f627c15d`  
		Last Modified: Thu, 23 Sep 2021 23:35:38 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
