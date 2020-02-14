<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `postgres`

-	[`postgres:10`](#postgres10)
-	[`postgres:10.12`](#postgres1012)
-	[`postgres:10.12-alpine`](#postgres1012-alpine)
-	[`postgres:10-alpine`](#postgres10-alpine)
-	[`postgres:11`](#postgres11)
-	[`postgres:11.7`](#postgres117)
-	[`postgres:11.7-alpine`](#postgres117-alpine)
-	[`postgres:11-alpine`](#postgres11-alpine)
-	[`postgres:12`](#postgres12)
-	[`postgres:12.2`](#postgres122)
-	[`postgres:12.2-alpine`](#postgres122-alpine)
-	[`postgres:12-alpine`](#postgres12-alpine)
-	[`postgres:9`](#postgres9)
-	[`postgres:9.4`](#postgres94)
-	[`postgres:9.4.26`](#postgres9426)
-	[`postgres:9.4.26-alpine`](#postgres9426-alpine)
-	[`postgres:9.4-alpine`](#postgres94-alpine)
-	[`postgres:9.5`](#postgres95)
-	[`postgres:9.5.21`](#postgres9521)
-	[`postgres:9.5.21-alpine`](#postgres9521-alpine)
-	[`postgres:9.5-alpine`](#postgres95-alpine)
-	[`postgres:9.6`](#postgres96)
-	[`postgres:9.6.17`](#postgres9617)
-	[`postgres:9.6.17-alpine`](#postgres9617-alpine)
-	[`postgres:9.6-alpine`](#postgres96-alpine)
-	[`postgres:9-alpine`](#postgres9-alpine)
-	[`postgres:alpine`](#postgresalpine)
-	[`postgres:latest`](#postgreslatest)

## `postgres:10`

```console
$ docker pull postgres@sha256:2aef165ab4f30fbb109e88959271d8b57489790ea13a77d27c02d8adb8feb20f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:10` - linux; amd64

```console
$ docker pull postgres@sha256:556411bc4fdc2e490e871b74d8de27285af3839bb975c96488dfaf82850273b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.6 MB (87585220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fea18bb7e20ab833902b993642c4f9404854675276843a458523cefef9c5f79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 06:07:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 06:07:31 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 06:07:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 06:07:59 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 06:08:00 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 06:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:08:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 06:08:12 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 06:09:09 GMT
ENV PG_MAJOR=10
# Sun, 02 Feb 2020 06:09:09 GMT
ENV PG_VERSION=10.11-1.pgdg90+1
# Sun, 02 Feb 2020 06:09:33 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 06:09:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 06:09:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 06:09:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sun, 02 Feb 2020 06:09:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 06:09:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 06:09:36 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 06:09:36 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:09:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 06:09:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:09:38 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 06:09:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0fe6664f6bb5f06d5d0a9a68c99a68be052403c684a8ffd98e70f6256d8ca`  
		Last Modified: Sun, 02 Feb 2020 06:12:59 GMT  
		Size: 4.5 MB (4501301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7ba8f77640450af762ebf643f368663949425d1bd516521dd9c0022a65461`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 1.8 KB (1779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1155d037e2c8553fc58b2671c2e61ca9ee29c7f712dbfc66dc20e8ab549c6b`  
		Last Modified: Sun, 02 Feb 2020 06:12:58 GMT  
		Size: 1.4 MB (1351457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febcfb7f8870017ab69faa0a454aa6a1e3cfde53c46074d1aa3e6edaea01adcc`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 6.2 MB (6182941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c78c79412b5cb255309e404e829646cc509a10cf8f55b2a5043da04d706604c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 295.6 KB (295582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a35744405c5f473d3002c5451970e6ff78bcc5eb330eea1c5595cca6b32679e`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27717922e0679badf783f2aa3179d254bb023533caf48d859c3d29723401701c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2e219af132dbb1e573652a6b6d83a6be04d749bfed7db1b682b9145603ab0e`  
		Last Modified: Sun, 02 Feb 2020 06:13:36 GMT  
		Size: 52.7 MB (52710259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b3ef20944e1d25af9286de2439921107cbe122aac2d2d2892401df5d14f6b2`  
		Last Modified: Sun, 02 Feb 2020 06:13:18 GMT  
		Size: 8.0 KB (8019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a9c306a963e258262299a1fd10cf95338d19c9a1f02ad366645067b074285d`  
		Last Modified: Sun, 02 Feb 2020 06:13:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef1baa10c10d014bd8d08712dc016c1d308b69d8abbb546924722730e80c0f4`  
		Last Modified: Sun, 02 Feb 2020 06:13:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b50bfdc61f5df6c587bdbdb49aadf266b3513adfc3ae5c027f405575f33517`  
		Last Modified: Sun, 02 Feb 2020 06:13:18 GMT  
		Size: 3.8 KB (3843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b7eb5dfc24ac106e63c186e180998963ad193cf4dd55e2196019005bb52bb8`  
		Last Modified: Sun, 02 Feb 2020 06:13:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; arm variant v5

```console
$ docker pull postgres@sha256:6f0bf700a6c7d78f4d6943098cde3951010d93ea1b3aa50647c373679f0d22a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.1 MB (84117037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3178651f7730e8c306e2655c0f3e68d47330af8dc2e0281c306d368b45c10a31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:53:57 GMT
ADD file:f0d179649cbf50028b5ecd832961cc332fb524c2f12fda6c8060c3c258208be6 in / 
# Sat, 01 Feb 2020 16:53:59 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:04:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 19:04:31 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 19:05:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 19:05:16 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 19:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 19:05:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 19:27:29 GMT
ENV PG_MAJOR=10
# Sat, 01 Feb 2020 19:27:30 GMT
ENV PG_VERSION=10.11-1.pgdg90+1
# Sat, 01 Feb 2020 19:48:35 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 19:48:39 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 19:48:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 19:48:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sat, 01 Feb 2020 19:48:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 19:48:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 19:48:46 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 19:48:47 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:48:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 19:48:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 19:48:50 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 19:48:50 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:03886a8604d1b5423798ee97917dcb9de4cfdfbb7c435a7988d5c5e69a78e3b7`  
		Last Modified: Sat, 01 Feb 2020 17:01:03 GMT  
		Size: 21.2 MB (21202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aaa01ea1502b56b5ebd804228ff2ea5ad2adf78d4797d7a6aa75903a7dc7a30`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 4.2 MB (4236888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feeb9ed754ebd60d2d8cdffa636ff7e5b6ea1b1f68fd7c7aac5f1dced2f8cf9`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142683156b4ad1e2209ecaac30f55cd1a7237fe046f545e7a64613b34c221671`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.3 MB (1311293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950d1d965477d4d1230281bd3043f7347d94e263cada82cd86f3f055cc269e93`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 6.2 MB (6185421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1690d5dc7daff0def912cfa3c22eff87c80edb8f734454280c116e5fd52ebb92`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 293.5 KB (293479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0191375b3084722e33f875137d737673fc3ec09776716614c4fcd6764e7884e`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9bf11db5cc7dd3ff01824ff16d5642657294a22e3ec2086a5b3575ef803947`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 4.8 KB (4791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a4c66da6bf116ddf6a1b199bb2a9f707649386ef012da5a1fa012e262858a2`  
		Last Modified: Sat, 01 Feb 2020 20:51:47 GMT  
		Size: 50.9 MB (50868054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def6a99605ef9524f50d32e318b43c965afd10c6e536d2a58270f2da07d79461`  
		Last Modified: Sat, 01 Feb 2020 20:51:25 GMT  
		Size: 8.0 KB (8025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3375e439d7ab1f1e74bf4582c399b4e97516edff91af3bd37735f1838a47044`  
		Last Modified: Sat, 01 Feb 2020 20:51:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbeef0e1abe19a95869162d9fefac57ae8acf3977ebbd59e77b4e9d8c90efc4`  
		Last Modified: Sat, 01 Feb 2020 20:51:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a835b4d5420c9c2ee740a87d519a8feb3cf71326f06df3984ec8b06640485bb`  
		Last Modified: Sat, 01 Feb 2020 20:51:25 GMT  
		Size: 3.8 KB (3843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293ead1f2f9b6784681f69ea655abe307cf241e21f6ecd74aff8d3a3c1ef1f1b`  
		Last Modified: Sat, 01 Feb 2020 20:51:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; arm variant v7

```console
$ docker pull postgres@sha256:0e42c1871116094b1d83bb9cf9860d8a5c825526ea0c086b00a6e4ab3121c318
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.2 MB (80248760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f39fb9ab868254f0fb80fe20bc0967bd5e983d366baa67ff1c800b5816000e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 08:58:06 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 08:58:07 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 08:58:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 08:58:44 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 08:58:45 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 08:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:58:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 08:59:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 09:19:58 GMT
ENV PG_MAJOR=10
# Sun, 02 Feb 2020 09:19:59 GMT
ENV PG_VERSION=10.11-1.pgdg90+1
# Sun, 02 Feb 2020 09:39:30 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 09:39:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 09:39:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 09:39:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sun, 02 Feb 2020 09:39:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 09:39:40 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 09:39:41 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 09:39:42 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:39:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 09:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:39:46 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 09:39:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e359f7642afed089b2d05ece4e0736e03ceb13a937f7478eb868702665f809`  
		Last Modified: Sun, 02 Feb 2020 10:36:41 GMT  
		Size: 3.9 MB (3872826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b5742cb7fbb2cdb38f99c354efd420d24d27dee9b21b232dc92100066c10b`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6852094413bd98c461152c87837e91176b94a6cadae25e1a31b7f07330ecc4`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.3 MB (1303620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589bd77312350a872d2ebc5a6638ec844bf3aece0160a35b34a5d5cf66ae0d22`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 6.2 MB (6185708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943e832035ee98c3689f148b48e73550099b8f81fe37da09aa6e1ae2ea1756ac`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 291.9 KB (291867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba8ac21d907e788e2f05af094077cd10bcd20b8bb6eb5021b9f01ae1cfb1d97`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f8d5c6112a73a87453a9f3b2c2c298c0d2c275026fb63fb5ecdd81e6205461`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 4.8 KB (4792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f698643b439ffded7d5c6aa6d05b601232099953b0f252226d3caf16a9742bb`  
		Last Modified: Sun, 02 Feb 2020 10:37:24 GMT  
		Size: 49.3 MB (49264053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0acbea3faf5cc1c6369e71baa3e85160f087e7553c7c856c1b40bba49fb4c1e`  
		Last Modified: Sun, 02 Feb 2020 10:37:04 GMT  
		Size: 8.0 KB (8023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a98542375a08552b49f4b24f62401f1ee6dd72a5b86bfbf1524b95f6326511`  
		Last Modified: Sun, 02 Feb 2020 10:37:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8925fbd3fb62d5ff202a4558a0009727643ae518950960c00d796e02c5b5d6bc`  
		Last Modified: Sun, 02 Feb 2020 10:37:05 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6740e525ea64be2e656d10d73edbf9dba7d9631b544dbee3c1d43306d3e65577`  
		Last Modified: Sun, 02 Feb 2020 10:37:04 GMT  
		Size: 3.8 KB (3845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7747ff09e9c90c866a38dad6ac3db87c9c2974a88c69019274523fd39d35d2c`  
		Last Modified: Sun, 02 Feb 2020 10:37:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:caa38ce8ee19729a1296e36792d443a40ef890d9c2ee35957587b13a0aa8971a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83115184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96f38b8b8028b22e8080bd9992297d36bb8453b06d4e762fe68082b716d87b6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:24:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 02:24:24 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 02:24:27 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 02:24:52 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 02:25:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 02:25:09 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 02:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:25:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 02:25:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 02:48:10 GMT
ENV PG_MAJOR=10
# Sun, 02 Feb 2020 02:48:12 GMT
ENV PG_VERSION=10.11-1.pgdg90+1
# Sun, 02 Feb 2020 03:08:06 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 03:08:13 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 03:08:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 03:08:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sun, 02 Feb 2020 03:08:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 03:08:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 03:08:20 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 03:08:21 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 03:08:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 03:08:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:08:26 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 03:08:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a29899232ff5984832260695109c206ed14783ab8a33dd8f593f40672e2cf51`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 4.1 MB (4077687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72390476b7ab26db4e6e224ad16f9c0a3d66dce6b4d9996f6edece0992dec78e`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4470eb370695bb8691186ee389e7be5deaeb4f0d84a84ca948ae39ea977a1`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.3 MB (1286440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b51db6dc34b50eff6b5d8120f3efff4e5269216d5ea5d004ce80782e7508411`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 6.2 MB (6185392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918217c35d15c52bb58861e8c65a6b6934bc554387043c67b630758273c41028`  
		Last Modified: Sun, 02 Feb 2020 04:07:20 GMT  
		Size: 292.1 KB (292139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea01905f4f686b651e994714cb840779b241fcf43c04c6cc2a0ae229543862dc`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ff0687a25d7e24b75be4e353f57d8821a81a4b8c51aff2a01f927bb70d1a76`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 4.8 KB (4794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400c3d418c6d066219182980461964218da5674d2cbe4eff368df59bc13a677e`  
		Last Modified: Sun, 02 Feb 2020 04:08:02 GMT  
		Size: 50.9 MB (50868600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfd8732d56bddb3a3e7476d4b9606bf1b7cfdcb863197ad77e38882a1b10204`  
		Last Modified: Sun, 02 Feb 2020 04:07:42 GMT  
		Size: 8.0 KB (8023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698fe3c901e353d406b2ef83c206f8bb7aef99ab8b833e7a4da3f4b5ad1b927e`  
		Last Modified: Sun, 02 Feb 2020 04:07:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fd774ecd778297fdabef32230b07beddf95486a8de4fa28ac9295278e3bcce`  
		Last Modified: Sun, 02 Feb 2020 04:07:42 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36de011b942bf3efd603800dde69fbc37fed4b02c4e2a7bc6f69a488a3c71273`  
		Last Modified: Sun, 02 Feb 2020 04:07:42 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aae9ab5aabe0316f6ffab96c3004527305c846faab3f6155c6f5ebad3d39b7`  
		Last Modified: Sun, 02 Feb 2020 04:07:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; 386

```console
$ docker pull postgres@sha256:f5e0c3ec5d2e4376f340b580b346e10da6a5f9fdfba58803fe235f71c586e8f2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.0 MB (88991216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb24217403f6a825c2b78146f00886f0d158fc191b6f9b853edf7aadf1783376`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:21:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:21:11 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:21:27 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:21:39 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:21:39 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:21:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:21:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:21:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:23:06 GMT
ENV PG_MAJOR=10
# Sat, 01 Feb 2020 21:23:06 GMT
ENV PG_VERSION=10.11-1.pgdg90+1
# Sat, 01 Feb 2020 21:23:46 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:23:48 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:23:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:23:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sat, 01 Feb 2020 21:23:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:23:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:23:52 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:23:52 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:23:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:23:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:23:54 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:23:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400715a0cf80a4163f9bdfb01029e10c149b8ff3ce6ef1248f400451f617b081`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 4.8 MB (4807817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57223b59a38681596adf27043fcaa0c4896293e4b8d488d81957c76d11ee0d7`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb13941b5f12a8251a7c85981cb0d44069be9f4d1644bc34a11ae761968abdd8`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.3 MB (1318016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ada6bc6e6f24824fc92e6f96abb0ec680d29443a640d4b03d2ac54a6cb74ba`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 6.2 MB (6182955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65761eaa1a3239dc440a674c9a27612170189ab04f41d5360678cc34ddfab827`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 296.8 KB (296752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81305139d5a6d74e0ed5bf9ba0163f5c6baf0c66890f74d05e94b5313a57d86e`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ff425a04fcdc853777162926c616c569257ea00e96154204e9e3f91e2f7527`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1712190452154d7741067ba7bff153e806a8cc7bcaf7383253582dd0b9da83d`  
		Last Modified: Sat, 01 Feb 2020 21:28:40 GMT  
		Size: 53.2 MB (53214566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f37fe3d7d805470d9b45c8227d4f1db0145811379ce4e8b502d4b410e5327`  
		Last Modified: Sat, 01 Feb 2020 21:28:14 GMT  
		Size: 8.0 KB (8018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243faad61a998f8d118a24e789060a94f58f93e18cb7adf415adce321d4cfc0b`  
		Last Modified: Sat, 01 Feb 2020 21:28:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be473c052ffeda07bff2833bc7594849752ed96a444b08f0bf7b0846b029a2b0`  
		Last Modified: Sat, 01 Feb 2020 21:28:14 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3bd8fc7ac5a0ac4564aba35aa3ba7782b25dcfd4c13ccc657b493ea2f3d337`  
		Last Modified: Sat, 01 Feb 2020 21:28:14 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8649553dd477c7b4e85f611d4e0436b771b455a4cdf9beba54c9e1f67fb207`  
		Last Modified: Sat, 01 Feb 2020 21:28:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; ppc64le

```console
$ docker pull postgres@sha256:4180c41dde3a1b3be585d9adf02086dab2d9ea3d5be0756041fb17fc521528ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87295133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe628a2cbca692fd7ffdaf49c27434a31de9a91cd8caa85fe944946ea736609b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:34:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 22:34:47 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 22:34:48 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 22:35:35 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 22:35:55 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 22:35:58 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 22:36:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:36:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 22:36:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:40:29 GMT
ENV PG_MAJOR=10
# Sat, 01 Feb 2020 22:40:32 GMT
ENV PG_VERSION=10.11-1.pgdg90+1
# Sat, 01 Feb 2020 22:43:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:43:51 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:44:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:44:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sat, 01 Feb 2020 22:44:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:44:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:44:24 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:44:26 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:44:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:44:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:44:40 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:44:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760805deb1a123f70f866680db67bfa3dcb8847b6ba0a19aa81db56e389e2fc0`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 4.4 MB (4364947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07edca5c09c7a639b08f5873160d9f51a67dca693c553c77bd4da3a487cf98b1`  
		Last Modified: Sat, 01 Feb 2020 22:57:59 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531ca140aa96954bbf71328b29b544b3a2e6d65750bde462ebaf5ceb9211a2f3`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 1.3 MB (1274917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5387f07d48aa567c90a5f600a88d52a3e23731fc526fe455615270e71eb87826`  
		Last Modified: Sat, 01 Feb 2020 22:57:57 GMT  
		Size: 6.2 MB (6185756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df00257572bca93ee8879d856b2ad35f675ee82aa6091ca73d467ca3743f67ed`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 293.5 KB (293536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d078612d1275942888b21d29cab572493f1e313c54b050434dcd70e2d76d544`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2e5ca1d60f37146aeff96ecb4c62cbe26cf5ebc72cb162751de46927921192`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9672d4d212b254165e4901f9cc49d73d0b9d3ba1bc9a010aab6b504813611fa`  
		Last Modified: Sat, 01 Feb 2020 22:58:34 GMT  
		Size: 52.4 MB (52356144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a959ae42d8fd57d7566e382374df7a33041ef2ab2ac1e4c4b1263aad86d525d`  
		Last Modified: Sat, 01 Feb 2020 22:58:18 GMT  
		Size: 8.0 KB (8022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc0dba8348eb026002a415168eee0aa496201187272c243bef72685b1ea0cdf`  
		Last Modified: Sat, 01 Feb 2020 22:58:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea9eb58814bb2229af4a4450044e7a688a50e963f98dc61ce82ee0677d71160`  
		Last Modified: Sat, 01 Feb 2020 22:58:19 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67eb21659abe308479d906519affecd0fd3b66af5642b150e96a8f7e7e3c100c`  
		Last Modified: Sat, 01 Feb 2020 22:58:19 GMT  
		Size: 3.8 KB (3845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28fde849e81dc5293c761b2000ad2d4b8e5542072accdad955d587641300aff`  
		Last Modified: Sat, 01 Feb 2020 22:58:18 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; s390x

```console
$ docker pull postgres@sha256:b679ae588cb304011db5548af06d052a96c34867f80af81f1104162ef1f7ec6b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87986965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:991cea5acf7d43212b7d6c696b8b20850e9192a84331e5224f9d34f2065cff02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:55 GMT
ADD file:cf4bb119f25d8a9b9a2cd43101d5e87e0dbaa42d3f6688b39e66eea637225cc2 in / 
# Sat, 01 Feb 2020 16:43:57 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:40:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:40:14 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:40:23 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:40:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:40:28 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:40:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:40:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:48:22 GMT
ENV PG_MAJOR=10
# Sat, 01 Feb 2020 21:48:22 GMT
ENV PG_VERSION=10.11-1.pgdg90+1
# Sat, 01 Feb 2020 21:55:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:55:17 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:55:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:55:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sat, 01 Feb 2020 21:55:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:55:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:55:19 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:55:19 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:55:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:55:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:55:20 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:55:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:24a7c24214752593c0f651c56554e1bc6056ce340eb46cb71ed7ff0c430845a8`  
		Last Modified: Sat, 01 Feb 2020 16:47:44 GMT  
		Size: 22.4 MB (22380184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba584ff8c21579486e3687e8a4f6d0ecc911f32353708e9693752a64526d34f8`  
		Last Modified: Sat, 01 Feb 2020 22:15:15 GMT  
		Size: 4.5 MB (4534611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437afaa09e73336a77de2eaf796fdf66bd35380394ac42d0840b500f8a4972df`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1625730f985442686e8bba703b5a2f74d8ebb56b6c3f09d255ee5520ae0b83a`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.3 MB (1340980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505f199fff79fe4eb15264a3e92774fffb954fa9ca0b399800fafb2991aba6ea`  
		Last Modified: Sat, 01 Feb 2020 22:15:13 GMT  
		Size: 6.2 MB (6209613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea830cdc46d22c2ae31a6b440834f2563d2e28b2548c24b1daac41d82482f5f4`  
		Last Modified: Sat, 01 Feb 2020 22:15:11 GMT  
		Size: 294.6 KB (294550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c761a50d986b42286d1616f6bb992a8469b97207f4b48e434a5b6a81e2fe6`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc1bb55d92f21306a95cb3259eec2a3f3659245aeebb728d6698b7be3381b8`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c320c2e3d6c23034755da98c9c63d323e5489f7fd3b760c1c77d1492890a92`  
		Last Modified: Sat, 01 Feb 2020 22:15:38 GMT  
		Size: 53.2 MB (53207955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9033eb3dbc5da55262daca572f15eae9d72c6ca54ac620a87e436f91d27ecf72`  
		Last Modified: Sat, 01 Feb 2020 22:15:28 GMT  
		Size: 8.0 KB (8022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e57be9507a1f098e7c24c3ba530ae6f11b018be1905bc10ff1932655b642d6d`  
		Last Modified: Sat, 01 Feb 2020 22:15:43 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f269c295bdc52923cd38e415be839fcb67c52bec04628afff5681d066ea0585d`  
		Last Modified: Sat, 01 Feb 2020 22:15:28 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9ec2fdc3457528198a85ada97bb14f8e358202df992842a58144266d4bf9e0`  
		Last Modified: Sat, 01 Feb 2020 22:15:44 GMT  
		Size: 3.8 KB (3845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6360b9dd1d882b06de4aa4f52850f721ed363628e43a0693585190427d7f8af9`  
		Last Modified: Sat, 01 Feb 2020 22:15:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:10.12`

**does not exist** (yet?)

## `postgres:10.12-alpine`

**does not exist** (yet?)

## `postgres:10-alpine`

```console
$ docker pull postgres@sha256:6f9e62f9d71757088980ec8e9828cfc912700b9b22936df3f8660d2691990fbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:10-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:890b7d0b68c94d414e6eecab7e5711b4e24c4901152f3ff628dbf2ccf02e3eef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28243929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb495265b81ffaa0d3bf8887231b954a1139b2e3d611c3ac3ddeaff72313909c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:19:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:19:59 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:31:08 GMT
ENV PG_MAJOR=10
# Thu, 30 Jan 2020 03:31:08 GMT
ENV PG_VERSION=10.11
# Thu, 30 Jan 2020 03:31:08 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 30 Jan 2020 03:34:00 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:34:01 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:34:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:34:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:34:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:34:03 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:34:03 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:34:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:34:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:34:04 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:34:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1030c456d04636112fa347ddc5296036cddf70c8085be2e3f3fb481898f18fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d0211bbd9a4fd28f739a797600d78394b15d947a30f55f70cfd5daf0f9e443`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f48353e3665648f8cd97643159bb8de43f4d02884c2b2a2525a50abc60bd53`  
		Last Modified: Thu, 30 Jan 2020 03:43:28 GMT  
		Size: 25.4 MB (25428005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce2b80cd483ab6dc702f2060736061315d61280d99318caa9ae5bb15c3603a5`  
		Last Modified: Thu, 30 Jan 2020 03:43:23 GMT  
		Size: 7.4 KB (7355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004ae34487bbdfbfebbbdb97e338a6d5b16bbcd4a4d2546adf5ba7b61db7f718`  
		Last Modified: Thu, 30 Jan 2020 03:43:23 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1576a1f3267b5d8254959a8d9cba7bf77e8b79b6edac801eea661f276d7dbfa3`  
		Last Modified: Thu, 30 Jan 2020 03:43:23 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ecb08b43cbff00a70ca6373f0f969eda2f0af0ddfb7214dfad17f3670ce2ed`  
		Last Modified: Thu, 30 Jan 2020 03:43:23 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9f4371ff641ee2bd46329be91fa78e564e82e40a537639ab63e2087f5c268c`  
		Last Modified: Thu, 30 Jan 2020 03:43:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:968e031903d7ebf4eefd192614682e0d45dc1af15f9512171fa5dfcd45587731
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.4 MB (27372853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f46d39f040bbc296201e29e500776e88193ff2b13dc97d2957271ce51a6c9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:49:35 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:49:36 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:49:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:58:56 GMT
ENV PG_MAJOR=10
# Thu, 30 Jan 2020 02:58:59 GMT
ENV PG_VERSION=10.11
# Thu, 30 Jan 2020 02:58:59 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 30 Jan 2020 03:01:54 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:01:57 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:02:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:02:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:02:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:02:09 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:02:10 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:02:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:02:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:02:13 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:02:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab27e2422be886bc0a338b0e0c20b8e2beea15b880defbac81f75c04495d0c2`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae2520a8d4cdac962b6d4a62335dce896f8ccb0b6d2693b0e72591fda026d14`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8819dd0e3fb4366b6a6539add738489fa9293635962d9e9070cc49e01e4f1cb8`  
		Last Modified: Thu, 30 Jan 2020 03:12:56 GMT  
		Size: 24.7 MB (24742202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a4eea7ca0c64d22711d191859210d21f12ea9c79614f0ac3c9e845d7f2d834`  
		Last Modified: Thu, 30 Jan 2020 03:12:46 GMT  
		Size: 7.4 KB (7353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead4c7a8854a30535a607bc2b580aeded481f7b6cc58672ee6515858de92584e`  
		Last Modified: Thu, 30 Jan 2020 03:12:46 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db9c3b873826f8850cf4a9b172308462b8730fa58e90f759dbb6b462af5e8bb`  
		Last Modified: Thu, 30 Jan 2020 03:12:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2595a39e25b4b00814fa6aeba01200eefbd0508a6addc00a0c59165c8eb06b7`  
		Last Modified: Thu, 30 Jan 2020 03:12:46 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c08476620ff849a114ea6ce057c4b91981c96a225167de984541fd3510eae8`  
		Last Modified: Thu, 30 Jan 2020 03:12:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:6009ad4d990d9b2562d92981937aa7140d0c1b8a191de96fe7f9f1043a569706
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.3 MB (26342827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1821924759fd823046cb4dacf7ab410727189e70cc8b073a2285020bc829d4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:00:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:00:13 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:00:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:07:34 GMT
ENV PG_MAJOR=10
# Thu, 30 Jan 2020 03:07:35 GMT
ENV PG_VERSION=10.11
# Thu, 30 Jan 2020 03:07:35 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 30 Jan 2020 03:09:58 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:10:03 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:10:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:10:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:10:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:10:08 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:10:08 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:10:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:10:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:10:11 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:10:12 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572777a7d0992ea05b14f2ba3230ce906c753dd21eb73ac2b6018551250312db`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8810228251d658112d3dbf2b9b1719f402a0c3477bf2eceaa5a20341bba3f5`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9535c66bbd54f3fc9d4f41b7219a7f21f512cf6260db0015411514df6cbd70c7`  
		Last Modified: Thu, 30 Jan 2020 03:19:50 GMT  
		Size: 23.9 MB (23910185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5780fbf19a452fa2cc34f98f81402bd57f79016dc3220f05f6c27fc8252948`  
		Last Modified: Thu, 30 Jan 2020 03:19:40 GMT  
		Size: 7.4 KB (7356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b55235ed1fc2ea5f815193d720e7ecf604ece58935d122ff1d6d7f746ec3d6`  
		Last Modified: Thu, 30 Jan 2020 03:19:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2333baf3d3eae8dd06e9cc96be0f85665a3bea36f7928ea3d856ae43722bb3be`  
		Last Modified: Thu, 30 Jan 2020 03:19:41 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b377a6d294097d64b8e34d474bd432aae1d2da2cce5a5cce5488a465f77ee4c`  
		Last Modified: Thu, 30 Jan 2020 03:19:41 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d119a8c70941da20b1b3c7af20299758f7e0e7f03fd1c1ac6bfbe5e20e385c11`  
		Last Modified: Thu, 30 Jan 2020 03:19:41 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:beeb097034292d977954865138f0fc7179954bfae54b37091f6f08ecb675726d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28020336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adbec5568df41a4a2c09fe79eb7dd37293d5d6246805a77594525d1cbbdfa8ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:40:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:40:28 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:47:41 GMT
ENV PG_MAJOR=10
# Thu, 30 Jan 2020 02:47:42 GMT
ENV PG_VERSION=10.11
# Thu, 30 Jan 2020 02:47:42 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 30 Jan 2020 02:50:16 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:50:20 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:50:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:50:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:50:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:50:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:50:27 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:50:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:50:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:50:30 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:50:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db837ff5778a13ace9e439e3bff33c317ecca84803a142a4ee4e05d2af54def`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92b445ab1ef4ba9a6120e5cc359b70cb88b74a46dee803f2709cb873a7be79`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d2a596d4e86c2efca64e2a17bbbca2293433c4d630e89cd10c98adf63675`  
		Last Modified: Thu, 30 Jan 2020 03:00:49 GMT  
		Size: 25.3 MB (25284173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42373a6f8d47890fc07fe27587a2b7ba33e384e7626197ec302e331d8b240910`  
		Last Modified: Thu, 30 Jan 2020 03:00:40 GMT  
		Size: 7.4 KB (7352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bf6c26848e1a2872ce24f5609190e575da0b9ef6c72be5fca4e2eec1e711ff`  
		Last Modified: Thu, 30 Jan 2020 03:00:41 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba2dc7ede45890fb79ef3c5221e3b3281ecd0f21b07e954d7b11d09ad85112e`  
		Last Modified: Thu, 30 Jan 2020 03:00:40 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac336583d3e9c763b5ecf14eab9e561eea59b69a6153947c17985199d6095cd`  
		Last Modified: Thu, 30 Jan 2020 03:00:41 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213a8c58c499163c4db30d9a24f44487f291387cf0ff4a476af074a078afd11c`  
		Last Modified: Thu, 30 Jan 2020 03:00:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; 386

```console
$ docker pull postgres@sha256:92f538f4aadcdac967ff9ef7f8e8eecd382a250308c99cac436b84dc700cb8ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29134182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78a582bfadd065c8d3dd5798ec72f01d2d4c70b1fdd4b4e3b1bfeb9233604efa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:38:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:38:44 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:38:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:52:09 GMT
ENV PG_MAJOR=10
# Thu, 30 Jan 2020 02:52:09 GMT
ENV PG_VERSION=10.11
# Thu, 30 Jan 2020 02:52:09 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 30 Jan 2020 02:55:58 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:55:58 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:55:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:55:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:56:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:56:00 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:56:01 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:56:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:56:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:56:02 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:56:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb8463eb063fd24e3d29bd4ca5b9ba1590717acda7415cb45da3e7560f0dd`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023c33adbfeb9b779f40edac1617b4514e1fb0b976b5b201dd0f7dc688f5e60`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880fdc15bbb701b95a163133d7302a0d65415afccfc1e5eb54379e3dbbd9101b`  
		Last Modified: Thu, 30 Jan 2020 03:08:03 GMT  
		Size: 26.3 MB (26314661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34c3643c6fc34720c5af29f5a32d9b7454cabeb44b290efce9ad95ae6d1c824`  
		Last Modified: Thu, 30 Jan 2020 03:07:55 GMT  
		Size: 7.4 KB (7351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d138897f98d7d67bb2ca0a5e896d23680b7c566eaec081ed5af8c8a82e9cf7`  
		Last Modified: Thu, 30 Jan 2020 03:07:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ca0e0c80e582c8749ff6e527066df318acf9d518696e8a6944a46bfa8a00d8`  
		Last Modified: Thu, 30 Jan 2020 03:07:55 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6575c474405af6550c05c3742fa327adb43a7ab4ccea0484223baef6086f7b96`  
		Last Modified: Thu, 30 Jan 2020 03:07:55 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e236b27b324830fac87dd9fa9b7d9023162f50b9822c38987452037615d7be52`  
		Last Modified: Thu, 30 Jan 2020 03:07:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:80ec147abbe2f07e0ffe559d0bd5bb2ccac9929b8b19cae718b887318d0cd48c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29336139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5837d2b74b0fcc43b49961d2d5c2b688bb3b07f23721f2a2d7179cd09960683d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:20:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:20:03 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:35:31 GMT
ENV PG_MAJOR=10
# Thu, 30 Jan 2020 03:35:34 GMT
ENV PG_VERSION=10.11
# Thu, 30 Jan 2020 03:35:38 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 30 Jan 2020 03:39:20 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:39:28 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:39:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:39:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:39:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:39:52 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:39:53 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:40:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:40:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:40:06 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:40:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8af198a4c612619984a3d16dc2a9fb3f15835dfbf5269a9eab9a345ed4f14`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852af7c4759ead6b82b170b6d34d124532026b41ec5d7dc4ec99bd6705f633a`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee4495c38e1524865f74c2aa5d1138d6308461f3571b9058e12815836380f66`  
		Last Modified: Thu, 30 Jan 2020 03:54:24 GMT  
		Size: 26.5 MB (26500923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d53f89a818eada380e664b9424b87b4c1889e36847ba8f9a89c1851a432d258`  
		Last Modified: Thu, 30 Jan 2020 03:54:15 GMT  
		Size: 7.3 KB (7350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277432fa34b11e0ddb60e679467f73943d59d0fd4532da36940e4af829c58bae`  
		Last Modified: Thu, 30 Jan 2020 03:54:15 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d86c6007ef484c415ed8a274fe9f39e5da065f6e594ed82ccaaafaccd2b989`  
		Last Modified: Thu, 30 Jan 2020 03:54:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6a0e6838876d4196203183a75708cee9b230d4b032475503423cb755da42b8`  
		Last Modified: Thu, 30 Jan 2020 03:54:15 GMT  
		Size: 3.8 KB (3840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa15da5d1a69b3b4778badf8ae5faffc6f9174a5d98836d06568eeb8f53f7c9`  
		Last Modified: Thu, 30 Jan 2020 03:54:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:eb9882c22ea02ed8feae8365d129584ce1bfad59eb7eb0dcae7b47f6376fa357
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (27990989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fef2ff12d9dd71cd2cfdb37684d2747498c56f15abdbd118cf468aabd1828c8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:48:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:48:56 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:48:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:57:09 GMT
ENV PG_MAJOR=10
# Thu, 30 Jan 2020 02:57:09 GMT
ENV PG_VERSION=10.11
# Thu, 30 Jan 2020 02:57:10 GMT
ENV PG_SHA256=0d5d14ff6b075655f4421038fbde3a5d7b418c26a249a187a4175600d7aecc09
# Thu, 30 Jan 2020 02:59:29 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:59:31 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:59:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:59:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:59:32 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:59:32 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:59:32 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:59:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:59:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:59:33 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:59:34 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d0ab56996305262d42136eee090848bbdf7cec28b8625e39078668b245db48`  
		Last Modified: Thu, 30 Jan 2020 03:07:31 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd3ab8f7e8df3f56e9628a504d2ea6db996a9910565bf84e3bc35bd847bcfb`  
		Last Modified: Thu, 30 Jan 2020 03:07:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871aec16983985363ddf58d97faa906335334a1c84063355db97b047e37bf4d9`  
		Last Modified: Thu, 30 Jan 2020 03:08:14 GMT  
		Size: 25.4 MB (25395868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb601ef1da6f031284d2a2b4c7323a6a2012e5b4c95fe94ddc5c83f6d369f976`  
		Last Modified: Thu, 30 Jan 2020 03:08:09 GMT  
		Size: 7.4 KB (7351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8623afdf36bf3c93d60144f903679334422a24ac55c7baa5b8e5a82d07d2fba`  
		Last Modified: Thu, 30 Jan 2020 03:08:09 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd18c98b63012553b7de396c4611bc10f7ea81a74785537bd4dbc6d42941044`  
		Last Modified: Thu, 30 Jan 2020 03:08:09 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8546db62dcd35b9f8a98e378ba05666286c4b0e280e6905ecf42128850cc1552`  
		Last Modified: Thu, 30 Jan 2020 03:08:14 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f9399f0158b0e2e883146cade4a12d8db7e22778a8fdedbf0adce6333cdc3b`  
		Last Modified: Thu, 30 Jan 2020 03:08:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:11`

```console
$ docker pull postgres@sha256:6f2062ab11d720f4756f17da4d0a64534346cce33b7cdea9d7ac4f43eed9fc02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:11` - linux; amd64

```console
$ docker pull postgres@sha256:a31620142b3532dfc32fa139693ed4a58c5fe6dba0496a1d8189f283c6455ad0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120853575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c963c0eb8c6efa49bb8352ea446f248d208d674cfc34fc9ea275b5f99f8dedd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 06:07:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 06:07:31 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 06:07:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 06:07:59 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 06:08:00 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 06:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:08:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 06:08:12 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 06:08:12 GMT
ENV PG_MAJOR=11
# Sun, 02 Feb 2020 06:08:12 GMT
ENV PG_VERSION=11.6-1.pgdg90+1
# Sun, 02 Feb 2020 06:08:52 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 06:08:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 06:08:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 06:08:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sun, 02 Feb 2020 06:08:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 06:08:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 06:08:57 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 06:08:57 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:08:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 06:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:08:59 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 06:08:59 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0fe6664f6bb5f06d5d0a9a68c99a68be052403c684a8ffd98e70f6256d8ca`  
		Last Modified: Sun, 02 Feb 2020 06:12:59 GMT  
		Size: 4.5 MB (4501301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7ba8f77640450af762ebf643f368663949425d1bd516521dd9c0022a65461`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 1.8 KB (1779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1155d037e2c8553fc58b2671c2e61ca9ee29c7f712dbfc66dc20e8ab549c6b`  
		Last Modified: Sun, 02 Feb 2020 06:12:58 GMT  
		Size: 1.4 MB (1351457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febcfb7f8870017ab69faa0a454aa6a1e3cfde53c46074d1aa3e6edaea01adcc`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 6.2 MB (6182941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c78c79412b5cb255309e404e829646cc509a10cf8f55b2a5043da04d706604c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 295.6 KB (295582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a35744405c5f473d3002c5451970e6ff78bcc5eb330eea1c5595cca6b32679e`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27717922e0679badf783f2aa3179d254bb023533caf48d859c3d29723401701c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e873db744a774fc090484a16444cd6c03fc24a491eae87a053a71796ec7fa`  
		Last Modified: Sun, 02 Feb 2020 06:13:13 GMT  
		Size: 86.0 MB (85978361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798bee0464b6a716ad504b02681bec33939edf666d09ae47539ae1a41fbf9507`  
		Last Modified: Sun, 02 Feb 2020 06:12:54 GMT  
		Size: 8.3 KB (8271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7ffb1fc147be7267eb2998ecd93792d9ba0c15cb6ad32ec65ab1bb2bce9f93`  
		Last Modified: Sun, 02 Feb 2020 06:12:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12e3b58e1821330947f1ef23a2f8afe6d384d3dfa6dd865227bb93c68db2450`  
		Last Modified: Sun, 02 Feb 2020 06:12:54 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f37fe16639a3bf19b800a62309e232d79d8d6f58f60d1796b80965e32015f72`  
		Last Modified: Sun, 02 Feb 2020 06:12:54 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbda5d3bd0266e01dedb2e0f285b6999ea1edf33148584ad3b323bca2466a988`  
		Last Modified: Sun, 02 Feb 2020 06:12:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; arm variant v5

```console
$ docker pull postgres@sha256:429a255a77216d934988a77351dd21bf7a04d5ad2bc0d65333b3e2f44357849a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84573918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81e28017e843f7e362bf2c9d775e2baa5974d92ac9d919116e4739a18309d103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:53:57 GMT
ADD file:f0d179649cbf50028b5ecd832961cc332fb524c2f12fda6c8060c3c258208be6 in / 
# Sat, 01 Feb 2020 16:53:59 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:04:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 19:04:31 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 19:05:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 19:05:16 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 19:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 19:05:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 19:05:38 GMT
ENV PG_MAJOR=11
# Sat, 01 Feb 2020 19:05:39 GMT
ENV PG_VERSION=11.6-1.pgdg90+1
# Sat, 01 Feb 2020 19:26:59 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 19:27:03 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 19:27:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 19:27:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sat, 01 Feb 2020 19:27:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 19:27:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 19:27:09 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 19:27:09 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:27:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 19:27:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 19:27:13 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 19:27:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:03886a8604d1b5423798ee97917dcb9de4cfdfbb7c435a7988d5c5e69a78e3b7`  
		Last Modified: Sat, 01 Feb 2020 17:01:03 GMT  
		Size: 21.2 MB (21202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aaa01ea1502b56b5ebd804228ff2ea5ad2adf78d4797d7a6aa75903a7dc7a30`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 4.2 MB (4236888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feeb9ed754ebd60d2d8cdffa636ff7e5b6ea1b1f68fd7c7aac5f1dced2f8cf9`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142683156b4ad1e2209ecaac30f55cd1a7237fe046f545e7a64613b34c221671`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.3 MB (1311293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950d1d965477d4d1230281bd3043f7347d94e263cada82cd86f3f055cc269e93`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 6.2 MB (6185421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1690d5dc7daff0def912cfa3c22eff87c80edb8f734454280c116e5fd52ebb92`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 293.5 KB (293479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0191375b3084722e33f875137d737673fc3ec09776716614c4fcd6764e7884e`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9bf11db5cc7dd3ff01824ff16d5642657294a22e3ec2086a5b3575ef803947`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 4.8 KB (4791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a7354f3303da2fd3f398606fafd88ab6d7a0d0e107b106d5c321a911b93cdc`  
		Last Modified: Sat, 01 Feb 2020 20:51:19 GMT  
		Size: 51.3 MB (51324683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08af6c3a3372f1a068489a055951eb04aafe9a2f15070d155b443ade9030aab4`  
		Last Modified: Sat, 01 Feb 2020 20:50:58 GMT  
		Size: 8.3 KB (8272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001402fe2a98438b93b6ab15da96bfde6a5db4d9a3dfac3a5c27947eb67b7a14`  
		Last Modified: Sat, 01 Feb 2020 20:50:58 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82ac80d8f2b223ed9208a5aa07a169d33f88bf580a21a524f24b529aa2a5fb6`  
		Last Modified: Sat, 01 Feb 2020 20:50:58 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b292dd007e928ebaff52120d93aec614f0cf080eb1f45ee6d0068749668252`  
		Last Modified: Sat, 01 Feb 2020 20:50:58 GMT  
		Size: 3.8 KB (3847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a72490ba47fa24e9859c7ce092fd1ee855b1c398fa9663ba76e0b20628abd0`  
		Last Modified: Sat, 01 Feb 2020 20:50:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; arm variant v7

```console
$ docker pull postgres@sha256:0a5e9cd138809a545843c34fd8e69958e1acdbe3c001ff742d8c4a3dfb3bcda4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80665193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85a4ec8f7ad4d42edaf512ba8477351d2b2a16d9847fe2dd29d7309073446b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 08:58:06 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 08:58:07 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 08:58:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 08:58:44 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 08:58:45 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 08:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:58:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 08:59:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 08:59:08 GMT
ENV PG_MAJOR=11
# Sun, 02 Feb 2020 08:59:09 GMT
ENV PG_VERSION=11.6-1.pgdg90+1
# Sun, 02 Feb 2020 09:19:16 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 09:19:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 09:19:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 09:19:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sun, 02 Feb 2020 09:19:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 09:19:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 09:19:29 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 09:19:30 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:19:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 09:19:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:19:38 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 09:19:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e359f7642afed089b2d05ece4e0736e03ceb13a937f7478eb868702665f809`  
		Last Modified: Sun, 02 Feb 2020 10:36:41 GMT  
		Size: 3.9 MB (3872826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b5742cb7fbb2cdb38f99c354efd420d24d27dee9b21b232dc92100066c10b`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6852094413bd98c461152c87837e91176b94a6cadae25e1a31b7f07330ecc4`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.3 MB (1303620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589bd77312350a872d2ebc5a6638ec844bf3aece0160a35b34a5d5cf66ae0d22`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 6.2 MB (6185708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943e832035ee98c3689f148b48e73550099b8f81fe37da09aa6e1ae2ea1756ac`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 291.9 KB (291867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba8ac21d907e788e2f05af094077cd10bcd20b8bb6eb5021b9f01ae1cfb1d97`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f8d5c6112a73a87453a9f3b2c2c298c0d2c275026fb63fb5ecdd81e6205461`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 4.8 KB (4792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d0f9ba3f1f4fcac08e01496644d3a536fbfef70a71b47fc24cdde54a72f399`  
		Last Modified: Sun, 02 Feb 2020 10:36:56 GMT  
		Size: 49.7 MB (49680235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb788e52833a66a159162712e6e6fca27cb2e08301d2c9e55ec25826535fcc7`  
		Last Modified: Sun, 02 Feb 2020 10:36:36 GMT  
		Size: 8.3 KB (8273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a05d0f244e12ba1fea3ede4effce833670eeabd575970a563d802b61a35dc4`  
		Last Modified: Sun, 02 Feb 2020 10:36:36 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fb91fef943b6cb9177916cac1b9d3de2c3ce032a42432b1a8387bac60d8ef6`  
		Last Modified: Sun, 02 Feb 2020 10:36:36 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0dbf1f3f235f85edad2bb4dbf57ca2fa63294cef3e1f6455ba957b98b12982`  
		Last Modified: Sun, 02 Feb 2020 10:36:36 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10231f921bee8c46395f1f2bc14697307b86397d8e04e6c1be83833130afcdb`  
		Last Modified: Sun, 02 Feb 2020 10:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:e3f0528d50604c17bc55a6779f77c6e2fd58987eba73597339f797484c8d6494
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83557910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7904724bd946e6e46b4c0c8d981dce2c80faf69f888fcb0ed3d991dd9357e593`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:24:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 02:24:24 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 02:24:27 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 02:24:52 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 02:25:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 02:25:09 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 02:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:25:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 02:25:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 02:25:35 GMT
ENV PG_MAJOR=11
# Sun, 02 Feb 2020 02:25:36 GMT
ENV PG_VERSION=11.6-1.pgdg90+1
# Sun, 02 Feb 2020 02:47:24 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 02:47:28 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 02:47:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 02:47:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sun, 02 Feb 2020 02:47:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 02:47:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 02:47:43 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 02:47:43 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 02:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 02:47:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 02:47:47 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 02:47:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a29899232ff5984832260695109c206ed14783ab8a33dd8f593f40672e2cf51`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 4.1 MB (4077687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72390476b7ab26db4e6e224ad16f9c0a3d66dce6b4d9996f6edece0992dec78e`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4470eb370695bb8691186ee389e7be5deaeb4f0d84a84ca948ae39ea977a1`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.3 MB (1286440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b51db6dc34b50eff6b5d8120f3efff4e5269216d5ea5d004ce80782e7508411`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 6.2 MB (6185392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918217c35d15c52bb58861e8c65a6b6934bc554387043c67b630758273c41028`  
		Last Modified: Sun, 02 Feb 2020 04:07:20 GMT  
		Size: 292.1 KB (292139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea01905f4f686b651e994714cb840779b241fcf43c04c6cc2a0ae229543862dc`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ff0687a25d7e24b75be4e353f57d8821a81a4b8c51aff2a01f927bb70d1a76`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 4.8 KB (4794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32188fa32d04978d8234b2cbe1d21cc62e1732aa7c4856829b2af078ab51eb0f`  
		Last Modified: Sun, 02 Feb 2020 04:07:35 GMT  
		Size: 51.3 MB (51311082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6146436326d947ef7d0e58cd7daf7cba6f2e000d749950cc4b958b133bb198`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 8.3 KB (8272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e02ff7aa9837aa0a6066930453b7c1cd2e53aac07ab7e331b45f5b2816c632e`  
		Last Modified: Sun, 02 Feb 2020 04:07:17 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857d8b11efaca299435bff7f3d1444728632e9e919f25f9f9bf8595242e841f0`  
		Last Modified: Sun, 02 Feb 2020 04:07:17 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae7c1b58fc30354cb32ec9012cef15fa356b237c921b60d92bc025e1350234b`  
		Last Modified: Sun, 02 Feb 2020 04:07:17 GMT  
		Size: 3.8 KB (3843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c159244105e86820db2f87ec1a4ccc627bd3f6a67f447103505b9e8e8f0947b`  
		Last Modified: Sun, 02 Feb 2020 04:07:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; 386

```console
$ docker pull postgres@sha256:85d79cba2d4942dad7c99f84ec389a5b9cc84fb07a3dcd3aff0fb06948cdc03b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124531032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6852e617fed4a781cc35feea11a73b64c8b06930be32e7df8d326afde0a415dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:21:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:21:11 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:21:27 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:21:39 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:21:39 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:21:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:21:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:21:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:21:53 GMT
ENV PG_MAJOR=11
# Sat, 01 Feb 2020 21:21:53 GMT
ENV PG_VERSION=11.6-1.pgdg90+1
# Sat, 01 Feb 2020 21:22:43 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:22:45 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:22:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:22:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sat, 01 Feb 2020 21:22:47 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:22:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:22:49 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:22:49 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:22:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:22:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:22:51 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:22:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400715a0cf80a4163f9bdfb01029e10c149b8ff3ce6ef1248f400451f617b081`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 4.8 MB (4807817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57223b59a38681596adf27043fcaa0c4896293e4b8d488d81957c76d11ee0d7`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb13941b5f12a8251a7c85981cb0d44069be9f4d1644bc34a11ae761968abdd8`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.3 MB (1318016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ada6bc6e6f24824fc92e6f96abb0ec680d29443a640d4b03d2ac54a6cb74ba`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 6.2 MB (6182955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65761eaa1a3239dc440a674c9a27612170189ab04f41d5360678cc34ddfab827`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 296.8 KB (296752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81305139d5a6d74e0ed5bf9ba0163f5c6baf0c66890f74d05e94b5313a57d86e`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ff425a04fcdc853777162926c616c569257ea00e96154204e9e3f91e2f7527`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab5535b08d16941898b8073471f2bd2b0eebe74b4d0aa5f6b5dca1290bf28b1`  
		Last Modified: Sat, 01 Feb 2020 21:28:09 GMT  
		Size: 88.8 MB (88754128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71df7678cb56fc07a1d968788cf318d24b7ccb4d457c2f519d71a8735fde2d3`  
		Last Modified: Sat, 01 Feb 2020 21:27:31 GMT  
		Size: 8.3 KB (8269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278e481aa671de40a527525d87c164c30547a71c298b6f4ca6b9014e84d539fb`  
		Last Modified: Sat, 01 Feb 2020 21:27:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a4bb82df5b6dd0daa24d0e010e66574de0e9b3a69051be6db6e717f947c73`  
		Last Modified: Sat, 01 Feb 2020 21:27:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17bbad3946b23a86aba6b4b28c303eab1d430c85c297d89dfac61013558bed`  
		Last Modified: Sat, 01 Feb 2020 21:27:31 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2fd044a2b19b7ad923ff03637fe56bcb093116d73fccb3ec2eb067d16ff075`  
		Last Modified: Sat, 01 Feb 2020 21:27:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; ppc64le

```console
$ docker pull postgres@sha256:fb4262dfc771913212a20c408033f58a899500e290f3a68385a7a666a1039ff0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87728962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fafb2c801f96ec6f132250dbee43423b81328e7ac7bbac1840b9855890f1857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:34:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 22:34:47 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 22:34:48 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 22:35:35 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 22:35:55 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 22:35:58 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 22:36:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:36:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 22:36:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:36:29 GMT
ENV PG_MAJOR=11
# Sat, 01 Feb 2020 22:36:31 GMT
ENV PG_VERSION=11.6-1.pgdg90+1
# Sat, 01 Feb 2020 22:39:27 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:39:36 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:39:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:39:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sat, 01 Feb 2020 22:39:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:39:55 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:39:58 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:40:00 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:40:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:40:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:40:12 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:40:15 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760805deb1a123f70f866680db67bfa3dcb8847b6ba0a19aa81db56e389e2fc0`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 4.4 MB (4364947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07edca5c09c7a639b08f5873160d9f51a67dca693c553c77bd4da3a487cf98b1`  
		Last Modified: Sat, 01 Feb 2020 22:57:59 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531ca140aa96954bbf71328b29b544b3a2e6d65750bde462ebaf5ceb9211a2f3`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 1.3 MB (1274917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5387f07d48aa567c90a5f600a88d52a3e23731fc526fe455615270e71eb87826`  
		Last Modified: Sat, 01 Feb 2020 22:57:57 GMT  
		Size: 6.2 MB (6185756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df00257572bca93ee8879d856b2ad35f675ee82aa6091ca73d467ca3743f67ed`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 293.5 KB (293536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d078612d1275942888b21d29cab572493f1e313c54b050434dcd70e2d76d544`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2e5ca1d60f37146aeff96ecb4c62cbe26cf5ebc72cb162751de46927921192`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd327e364f0db66a42041ba16cac03f2a4f04fe0040b2c07f1022acbeba5288`  
		Last Modified: Sat, 01 Feb 2020 22:58:08 GMT  
		Size: 52.8 MB (52789720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1669f9b2963e3ac665ffadd19e800c2f2aa60d76b099d61dc57b2166aa4d0880`  
		Last Modified: Sat, 01 Feb 2020 22:57:50 GMT  
		Size: 8.3 KB (8275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa087ef1a9af7cb587af85cdd13a52066338b064c51dcd5179973fa4a42bd2c4`  
		Last Modified: Sat, 01 Feb 2020 22:57:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478f4723cedc5a8119d1771b88b813b4e86a3197b231d3a6fe7e950b2140f511`  
		Last Modified: Sat, 01 Feb 2020 22:57:51 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dbd8bc635132dd653b14059cde6e32cf855c6732a0a60adf2633ab8e94dc6f`  
		Last Modified: Sat, 01 Feb 2020 22:57:50 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2892cf7270cd889af47fe1b81426967e25c8a5fc9e016b7423b74501bae440`  
		Last Modified: Sat, 01 Feb 2020 22:57:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; s390x

```console
$ docker pull postgres@sha256:7ec8058e9367b3ffe1905aabe14fc9d0621d6cb133bd3f2ef99f0e96f115f28d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88430602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de059a1f296b5bb7467cfe92594fa901d72c52c408097432654c1c8f21f747c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:55 GMT
ADD file:cf4bb119f25d8a9b9a2cd43101d5e87e0dbaa42d3f6688b39e66eea637225cc2 in / 
# Sat, 01 Feb 2020 16:43:57 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:40:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:40:14 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:40:23 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:40:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:40:28 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:40:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:40:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:40:35 GMT
ENV PG_MAJOR=11
# Sat, 01 Feb 2020 21:40:35 GMT
ENV PG_VERSION=11.6-1.pgdg90+1
# Sat, 01 Feb 2020 21:47:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:47:58 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:47:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:47:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Sat, 01 Feb 2020 21:47:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:47:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:48:00 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:48:00 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:48:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:48:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:48:01 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:48:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:24a7c24214752593c0f651c56554e1bc6056ce340eb46cb71ed7ff0c430845a8`  
		Last Modified: Sat, 01 Feb 2020 16:47:44 GMT  
		Size: 22.4 MB (22380184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba584ff8c21579486e3687e8a4f6d0ecc911f32353708e9693752a64526d34f8`  
		Last Modified: Sat, 01 Feb 2020 22:15:15 GMT  
		Size: 4.5 MB (4534611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437afaa09e73336a77de2eaf796fdf66bd35380394ac42d0840b500f8a4972df`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1625730f985442686e8bba703b5a2f74d8ebb56b6c3f09d255ee5520ae0b83a`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.3 MB (1340980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505f199fff79fe4eb15264a3e92774fffb954fa9ca0b399800fafb2991aba6ea`  
		Last Modified: Sat, 01 Feb 2020 22:15:13 GMT  
		Size: 6.2 MB (6209613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea830cdc46d22c2ae31a6b440834f2563d2e28b2548c24b1daac41d82482f5f4`  
		Last Modified: Sat, 01 Feb 2020 22:15:11 GMT  
		Size: 294.6 KB (294550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c761a50d986b42286d1616f6bb992a8469b97207f4b48e434a5b6a81e2fe6`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc1bb55d92f21306a95cb3259eec2a3f3659245aeebb728d6698b7be3381b8`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68100f391b51fbbdb755e43d37ead2b0496364721d04a1a8293f1c6574dadcf7`  
		Last Modified: Sat, 01 Feb 2020 22:15:21 GMT  
		Size: 53.7 MB (53651347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc2c80357c9c1855fc0c9841343193a047c37a3fcab8a6ac9c7c48469cd5cf5`  
		Last Modified: Sat, 01 Feb 2020 22:15:09 GMT  
		Size: 8.3 KB (8273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54ced45333b18ecea3eae89a2a1051a7ec911317a407ce000a164d66044a59c`  
		Last Modified: Sat, 01 Feb 2020 22:15:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d8f178a8faa4c847729844cd6575f1b49748eb6b7d51b94a0104b19076b54c`  
		Last Modified: Sat, 01 Feb 2020 22:15:24 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037a796b80087b6c5f12b817dd9dab293209624ab21478571b001ddae7609109`  
		Last Modified: Sat, 01 Feb 2020 22:15:09 GMT  
		Size: 3.8 KB (3843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f8ed340c443c83acb13474b66a81ce0c5300f17e261102dd36b7e60e9f29a6`  
		Last Modified: Sat, 01 Feb 2020 22:15:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:11.7`

**does not exist** (yet?)

## `postgres:11.7-alpine`

**does not exist** (yet?)

## `postgres:11-alpine`

```console
$ docker pull postgres@sha256:c132d7802dcc127486a403fb9e9a52d9df2e3ab84037c5de8395ed6ba2743e20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:11-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:b262fc1e6a8c0dfc86a31d15dc9400d153fc79f236a2dadc5d44bb2ccc4c6e6b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.2 MB (59224943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ae06c2ad76783e0775c1e7b8ab12c78a695e4075aef935fadb3c177e272168`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:19:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:19:59 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:25:33 GMT
ENV PG_MAJOR=11
# Thu, 30 Jan 2020 03:25:33 GMT
ENV PG_VERSION=11.6
# Thu, 30 Jan 2020 03:25:33 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 30 Jan 2020 03:30:45 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:30:46 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:30:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:30:47 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:30:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:30:48 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:30:48 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:30:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:30:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:30:49 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:30:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1030c456d04636112fa347ddc5296036cddf70c8085be2e3f3fb481898f18fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d0211bbd9a4fd28f739a797600d78394b15d947a30f55f70cfd5daf0f9e443`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d0560c0a3f2c59167ef3b78ef5baae91ce5f8ed2d2c4cc2f1b6349ef0e7703`  
		Last Modified: Thu, 30 Jan 2020 03:43:19 GMT  
		Size: 56.4 MB (56408808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7fd4584a5f30702665120db98e70b258754b6b209e7aa5a01db49b0c54486c`  
		Last Modified: Thu, 30 Jan 2020 03:43:10 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63eb0325fe1cb0092eb70e481574d5708532a88bbb3bb57bd433f8f8d723513f`  
		Last Modified: Thu, 30 Jan 2020 03:43:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67486507716c0761ea8f4d113125b6732ffd57c189a0465a461fbdb1b059133`  
		Last Modified: Thu, 30 Jan 2020 03:43:09 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58de2b85820aeb8be4a28742feb0168ad59b7f8016e2210ba30cb55129f4482`  
		Last Modified: Thu, 30 Jan 2020 03:43:09 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca982626dd56ebba8888775906087b42e7c22ae8718c1b22b469f0be57c54265`  
		Last Modified: Thu, 30 Jan 2020 03:43:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:9a428e976f67ed6d8e7c781aaeefa7f140da5f42bc9765e9441a98bdb408f1d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57585599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c778420aaf9dbda5c29edf6a4c51c278cbbdbe2dd5ad4235b47c7f0c30604bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:49:35 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:49:36 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:49:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:54:24 GMT
ENV PG_MAJOR=11
# Thu, 30 Jan 2020 02:54:25 GMT
ENV PG_VERSION=11.6
# Thu, 30 Jan 2020 02:54:26 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 30 Jan 2020 02:58:34 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:58:39 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:58:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:58:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:58:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:58:45 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:58:46 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:58:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:58:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:58:49 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:58:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab27e2422be886bc0a338b0e0c20b8e2beea15b880defbac81f75c04495d0c2`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae2520a8d4cdac962b6d4a62335dce896f8ccb0b6d2693b0e72591fda026d14`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8eb0589423f02b30c433f815eb5639a2fbf86e2dc190caa377f4b6d47a8c6f`  
		Last Modified: Thu, 30 Jan 2020 03:12:38 GMT  
		Size: 55.0 MB (54954730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf9888e34161ea7beb81433a0a5c435d58d40264a71d2f5e88bd93a0ce0c18a`  
		Last Modified: Thu, 30 Jan 2020 03:12:18 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b72cfda5cd795ac75b7ff7edb519215cc22988a3acc969cdc97cf6cd1d42636`  
		Last Modified: Thu, 30 Jan 2020 03:12:18 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc46604dea47a5ea5b1a3e08cf37905020d0e9b41ba96f4d17cd4199cabca44`  
		Last Modified: Thu, 30 Jan 2020 03:12:18 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5ecf51b5a3a48b9644d97d00e85f83cd24cea88c79211922eb685a2df7b0f4`  
		Last Modified: Thu, 30 Jan 2020 03:12:18 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7256c4bd9e7c09e74b64778710434a25e14c8450d300ff14f8312b47ca498bc7`  
		Last Modified: Thu, 30 Jan 2020 03:12:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:c4baced0792c50f01d6feadb78bd8b12971ad8886e30d73f467a6b747b933494
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54868847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8a65a952c637ee89aca804e1409b65b7974da404a24c97c9ed97b91c10d3fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:00:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:00:13 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:00:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:03:58 GMT
ENV PG_MAJOR=11
# Thu, 30 Jan 2020 03:03:59 GMT
ENV PG_VERSION=11.6
# Thu, 30 Jan 2020 03:03:59 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 30 Jan 2020 03:07:02 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:07:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:07:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:07:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:07:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:07:10 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:07:11 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:07:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:07:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:07:14 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:07:15 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572777a7d0992ea05b14f2ba3230ce906c753dd21eb73ac2b6018551250312db`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8810228251d658112d3dbf2b9b1719f402a0c3477bf2eceaa5a20341bba3f5`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebe58a6169eac7e6b824be739891d1d4d5da517b99bd426387df6cfe269d70d`  
		Last Modified: Thu, 30 Jan 2020 03:19:16 GMT  
		Size: 52.4 MB (52435992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65459fe5cadc51b067769589bb46745545f38cee9361b86f74edfb55bf696950`  
		Last Modified: Thu, 30 Jan 2020 03:19:00 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d648a43cb1291ba622d326b707953d08e391fc7abc21d49713e1b901857755bb`  
		Last Modified: Thu, 30 Jan 2020 03:19:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b77a0cc188e60fc4507a55cee49c29114992ef54535955803f9603dae65e3c`  
		Last Modified: Thu, 30 Jan 2020 03:19:00 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb9395e0678f6b5239ad96c5aec762f93c55d674f2ff4c56313519b9acd030e`  
		Last Modified: Thu, 30 Jan 2020 03:19:01 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128b23d2433809066293bda6598ed88acc7ed1d96655adaaeae2041473b8c634`  
		Last Modified: Thu, 30 Jan 2020 03:19:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:dc3bc6c3db1d8c98fac618615827274d1cff18ba260413f8f2b3a7f22b333bf6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58821062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94d455984111c9a4c73593a1eeb21d423f2452d0b32ed1d8959c4bd84d18b722`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:40:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:40:28 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:44:03 GMT
ENV PG_MAJOR=11
# Thu, 30 Jan 2020 02:44:04 GMT
ENV PG_VERSION=11.6
# Thu, 30 Jan 2020 02:44:04 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 30 Jan 2020 02:47:04 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:47:07 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:47:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:47:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:47:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:47:11 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:47:12 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:47:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:47:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:47:15 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:47:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db837ff5778a13ace9e439e3bff33c317ecca84803a142a4ee4e05d2af54def`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92b445ab1ef4ba9a6120e5cc359b70cb88b74a46dee803f2709cb873a7be79`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be764112c601752cb4e02e9b43b2d1f7bb3f5bdc12b401ad15d7e7086963c4d5`  
		Last Modified: Thu, 30 Jan 2020 03:00:34 GMT  
		Size: 56.1 MB (56084683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb2c374970a3ce084b072c74382dea4001896c8f1e1b9d811ed7b834fa15a70`  
		Last Modified: Thu, 30 Jan 2020 03:00:13 GMT  
		Size: 7.6 KB (7571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161881585d5ee1df5055a4322c79d80b367f7191bd1a6c5039aacfc462724fab`  
		Last Modified: Thu, 30 Jan 2020 03:00:13 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd7e73537f6a0a3a59d229201ed45aa5c197d286cecc6573748cd9d09774eaf`  
		Last Modified: Thu, 30 Jan 2020 03:00:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5e526c2d858c8ce0851f8d116cb5b8a0b124205ff3c7f4dc3e98d1ffe77c66`  
		Last Modified: Thu, 30 Jan 2020 03:00:13 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a186f0dc02121261aa92ee0081cc1eb3000c016ade13e7d5169cd3ae56040408`  
		Last Modified: Thu, 30 Jan 2020 03:00:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; 386

```console
$ docker pull postgres@sha256:e98706031f6463887844146c97bec2623559b49d0b1e4d5540f19abe229ddfcb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62422293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:746ad5ec11410ca458ad5ade59ff282695fbb9ca4c50ec4149f2bcad17b5b283`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:38:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:38:44 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:38:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:45:34 GMT
ENV PG_MAJOR=11
# Thu, 30 Jan 2020 02:45:34 GMT
ENV PG_VERSION=11.6
# Thu, 30 Jan 2020 02:45:34 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 30 Jan 2020 02:51:50 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:51:51 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:51:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:51:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:51:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:51:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:51:53 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:51:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:51:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:51:54 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:51:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb8463eb063fd24e3d29bd4ca5b9ba1590717acda7415cb45da3e7560f0dd`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023c33adbfeb9b779f40edac1617b4514e1fb0b976b5b201dd0f7dc688f5e60`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1243f332516ec68665ee697498e9db0c5729810ac50702dc3adbe9d8b2c7f3e7`  
		Last Modified: Thu, 30 Jan 2020 03:07:52 GMT  
		Size: 59.6 MB (59602552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378365d8cd350708f2fc3ba6435cd23e6ef1755cdcf3de9315f2d429d017825b`  
		Last Modified: Thu, 30 Jan 2020 03:07:38 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cec2f865da5138e7786c59aa52eae04c53722c39ecbbe81db3300bede7392c`  
		Last Modified: Thu, 30 Jan 2020 03:07:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db85be9a79188f794edc2afd1c689e2bd296fe64226843eb4ad775c188fbbe5c`  
		Last Modified: Thu, 30 Jan 2020 03:07:38 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df84d57474fc3ab8c27263c92818a60d66a0d42584072afa670ed60377160c4`  
		Last Modified: Thu, 30 Jan 2020 03:07:38 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c8cb60a57160521aae31fec935a9fb4c28644966f97075f1be0cb04234fe2a`  
		Last Modified: Thu, 30 Jan 2020 03:07:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:7d0f690c667b86d8e626f12990f8d374dcf691fdbd1e612d9020ed5805da1694
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61452543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b4b3bee7c94824e41b03781adc6722ef4cd11fd42ee77e4ff53f155268593d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:20:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:20:03 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:29:13 GMT
ENV PG_MAJOR=11
# Thu, 30 Jan 2020 03:29:14 GMT
ENV PG_VERSION=11.6
# Thu, 30 Jan 2020 03:29:17 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 30 Jan 2020 03:34:15 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:34:23 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:34:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:34:34 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:34:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:34:48 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:34:51 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:35:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:35:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:35:07 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:35:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8af198a4c612619984a3d16dc2a9fb3f15835dfbf5269a9eab9a345ed4f14`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852af7c4759ead6b82b170b6d34d124532026b41ec5d7dc4ec99bd6705f633a`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbf3f3dce0ff079f24314480819f8c2a2fac2a7ffa8d89d8292f8cdabff7197`  
		Last Modified: Thu, 30 Jan 2020 03:54:05 GMT  
		Size: 58.6 MB (58617108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04b02161bd0be2a1c49b659b180c53a664ab480a5ff0c34477d82769c66b787`  
		Last Modified: Thu, 30 Jan 2020 03:53:50 GMT  
		Size: 7.6 KB (7571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c5eb02148e0c88c7eb87b9fdb5f6f0d326ca43f1fa2ad679b4e3e3804c5279`  
		Last Modified: Thu, 30 Jan 2020 03:53:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4c9a06c46bfc507abae73604bf07f232e6307266994f0b684cb7336859f48c`  
		Last Modified: Thu, 30 Jan 2020 03:53:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0970d6c6861bb2bc1d597bff68c7be58e8f7ccd4a0441c379f8f0db50c1879`  
		Last Modified: Thu, 30 Jan 2020 03:53:49 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697ab8cc403969f071ef85aa775f23299ba83346997871d98bda39e3505c6e6e`  
		Last Modified: Thu, 30 Jan 2020 03:53:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:fd02fb10c39bf6ed92fb12b5517981635c123082849d5de2fc07c9cfdfd4ce76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61172188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0e9c430afcfca2cd9a7a82282793ee02f26878fb70144abf75501405b70897`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:48:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:48:56 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:48:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:53:02 GMT
ENV PG_MAJOR=11
# Thu, 30 Jan 2020 02:53:02 GMT
ENV PG_VERSION=11.6
# Thu, 30 Jan 2020 02:53:02 GMT
ENV PG_SHA256=49924f7ff92965fdb20c86e0696f2dc9f8553e1563124ead7beedf8910c13170
# Thu, 30 Jan 2020 02:56:45 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:56:48 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:56:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:56:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:56:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:56:49 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:56:50 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:56:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:56:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:56:51 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:56:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d0ab56996305262d42136eee090848bbdf7cec28b8625e39078668b245db48`  
		Last Modified: Thu, 30 Jan 2020 03:07:31 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd3ab8f7e8df3f56e9628a504d2ea6db996a9910565bf84e3bc35bd847bcfb`  
		Last Modified: Thu, 30 Jan 2020 03:07:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cffd9b39aae873e62cf37d8ec910161cd463cce370f404ba14ec88b3006523a`  
		Last Modified: Thu, 30 Jan 2020 03:07:58 GMT  
		Size: 58.6 MB (58576850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a650aff9d6e5521b072b59d9a55fa1c85d717a34bb2dc6c806458b1247c5911`  
		Last Modified: Thu, 30 Jan 2020 03:07:49 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b956ef2854c93a076973bd2e462f814c0bbddd89ed49c611e65b477675daa052`  
		Last Modified: Thu, 30 Jan 2020 03:08:04 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6fd5895486f011267bd72d82d4a350740723c00f98fc77720663a705c7effa`  
		Last Modified: Thu, 30 Jan 2020 03:07:49 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef092b0802ef6f805a414a8a6f26e8a408c50968fe13e029f2b09645677f186`  
		Last Modified: Thu, 30 Jan 2020 03:07:49 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21be8be24fa564d0fb205dd155806ad144b0fbe4ee1acf87a35393e86ffc1bde`  
		Last Modified: Thu, 30 Jan 2020 03:08:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:12`

```console
$ docker pull postgres@sha256:5181eccc7c903e4f1beffa89a735cb7ed72e0c81d6c34c471552c3fa8bff0858
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:12` - linux; amd64

```console
$ docker pull postgres@sha256:0d4312223e13e5282f99d413950aa35cd624999a8650ad088095fe50e412e0b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132459661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf879a45faaacd2806705321f157c4c77682c7599589fed65d80f19bb61615a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:05:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 06:05:57 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 06:05:57 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 06:06:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 06:06:21 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 06:06:22 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 06:06:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:06:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 06:06:31 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 06:06:31 GMT
ENV PG_MAJOR=12
# Sun, 02 Feb 2020 06:06:32 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sun, 02 Feb 2020 06:07:06 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 06:07:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 06:07:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 06:07:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sun, 02 Feb 2020 06:07:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 06:07:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 06:07:09 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 06:07:09 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:07:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 06:07:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:07:10 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 06:07:11 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b355dbb6c6ba49b1944319de07e58ca26244ec451633b9d7656e77d0df4b8b`  
		Last Modified: Sun, 02 Feb 2020 06:12:26 GMT  
		Size: 4.2 MB (4177987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d237363a1a91586c6e1ad9d62722a3d56ca984ba9f2873e138e8085acb6ea140`  
		Last Modified: Sun, 02 Feb 2020 06:12:24 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b9d2fde66f1f78cc87ed21cdb8b3baa700c780dc2fe92fcc012cb8a4e1f66`  
		Last Modified: Sun, 02 Feb 2020 06:12:24 GMT  
		Size: 1.4 MB (1358574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646492d166e7a9b48cc30447d45f13c7738076910bf6f30819aeeaa291810d33`  
		Last Modified: Sun, 02 Feb 2020 06:12:27 GMT  
		Size: 8.0 MB (7964389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eeac6fd5fb8c3b933413c46ab8c37dd54763a866a5a4191a946b4f5e4f7f6d`  
		Last Modified: Sun, 02 Feb 2020 06:12:22 GMT  
		Size: 300.9 KB (300940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502963de6da85420287fa1c54411e4fa45a266d8cde698de5b962b3f02ab833d`  
		Last Modified: Sun, 02 Feb 2020 06:12:22 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7263f7627b9115c61347a0c10dd3ad98c8986878b1dba57276af6ce68d2a982`  
		Last Modified: Sun, 02 Feb 2020 06:12:22 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b135c7e429e5c80eb1930f02813862068f82563fea9acf9c0e9cbd86e2aba7`  
		Last Modified: Sun, 02 Feb 2020 06:12:49 GMT  
		Size: 91.5 MB (91547373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259a29a883ed61840fae1401f7af8f330a72e1b65c41d5f730df92429cdce564`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 8.9 KB (8945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b8f133c3f497f82fa1d3a8a59ed3f7d00f5aa9c7935a703d740b56710eb9a6`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e91678bd481c43532c7a173153bcecc0aea53dd55eef51e073a15b6808c88f`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15326bd3db004029e30f63c6193c06324af0d60d72e756195b3c62d2d3d65e23`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aab6409ca4d25a8800cce887ab77be76cb19c699522dcbb430e9ba38b653746`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; arm variant v5

```console
$ docker pull postgres@sha256:e078eadc94b2b3179a43131b2ff17b09eb955d643c354aaf5a416d6a19f0890d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126421019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5426b72e8515ab0aaa576a6eeedf6eeb7b0267a5310a02106b3e8f5859597d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:35:01 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 18:35:02 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 18:35:23 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:35:44 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 18:35:46 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 18:35:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 18:36:01 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 18:36:02 GMT
ENV PG_MAJOR=12
# Sat, 01 Feb 2020 18:36:03 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sat, 01 Feb 2020 19:03:36 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 19:03:41 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 19:03:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 19:03:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 01 Feb 2020 19:03:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 19:03:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 19:03:46 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 19:03:47 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:03:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 19:03:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 19:03:50 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 19:03:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70006e2ae692e3a1d3eda514f0de630b9cd77673aeb976c1e8a02b73cf8b7264`  
		Last Modified: Sat, 01 Feb 2020 20:50:23 GMT  
		Size: 3.8 MB (3847808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51f7983f9190b3cf57e2162aaa536103797b7b2db41ec034ac1b7bb738a7db4`  
		Last Modified: Sat, 01 Feb 2020 20:50:22 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f43bd19defefde17a52fb094b49664f52f5d36d08e761452ab81b6daf3d2469`  
		Last Modified: Sat, 01 Feb 2020 20:50:22 GMT  
		Size: 1.3 MB (1318116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bee3c68ffa27d48c5e64724a11c9ce65500c467e37cd40b9d40bf6f7e7e08d`  
		Last Modified: Sat, 01 Feb 2020 20:50:24 GMT  
		Size: 8.0 MB (7965055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df868ae33379c795c154a8ddcc37740d3b7f827af475b18c68884116d795a66d`  
		Last Modified: Sat, 01 Feb 2020 20:50:20 GMT  
		Size: 298.7 KB (298736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6934c8d464038d8a2d408d443259cd545bbd9ffcb8ceab0dbb2342f96ab69711`  
		Last Modified: Sat, 01 Feb 2020 20:50:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520c13f9b7c083374a70fe0f3325f0bcb4088a5b3417e1c9bb794849aa00aa2e`  
		Last Modified: Sat, 01 Feb 2020 20:50:20 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90083940f769eb064647115deaab33448ab82d0c883c8a7e2e524135927d3e72`  
		Last Modified: Sat, 01 Feb 2020 20:50:49 GMT  
		Size: 88.1 MB (88143396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4f7f8266b1cda46a0d14eda5bc4bc6f097081c177b2cfc5037390692b136ba`  
		Last Modified: Sat, 01 Feb 2020 20:50:18 GMT  
		Size: 8.9 KB (8946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3c53c89257271a5f68c228e3cb27b34fca81d0c9ca4a5d434980c5bc52a8c1`  
		Last Modified: Sat, 01 Feb 2020 20:50:18 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b423b27e12af4ee04ae7a8fc7412ade0b6715816f633009fb0a3f1a361579631`  
		Last Modified: Sat, 01 Feb 2020 20:50:18 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00935b7e8f2d0afee05a0c6998f6111a1ae415e39e8c0c9ffe6dab1d0b726ba5`  
		Last Modified: Sat, 01 Feb 2020 20:50:19 GMT  
		Size: 3.8 KB (3833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2df8f298ce648d91a02e60522608117d44a826a68b45d09b962d07a279dc3f`  
		Last Modified: Sat, 01 Feb 2020 20:50:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; arm variant v7

```console
$ docker pull postgres@sha256:7ccf4bc46e42d9279f0a20dd890c4b50d14a1fa42d0091346f7305ab09c8b0df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121935162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc1644763b76d135d79b7c008799fada6975721de94086a79e17d419baa2831a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:30:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 08:30:25 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 08:30:26 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 08:30:45 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 08:31:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 08:31:06 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 08:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:31:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 08:31:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 08:31:25 GMT
ENV PG_MAJOR=12
# Sun, 02 Feb 2020 08:31:26 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sun, 02 Feb 2020 08:57:06 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 08:57:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 08:57:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 08:57:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sun, 02 Feb 2020 08:57:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 08:57:21 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 08:57:22 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 08:57:23 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 08:57:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 08:57:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 08:57:26 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 08:57:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d581d588bd5e2ca7c84216a9def839421358d391a572f06f6a6397329cd2e429`  
		Last Modified: Sun, 02 Feb 2020 10:35:59 GMT  
		Size: 3.5 MB (3481690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d38b43f6d701f50e329b3c3adb68cd87e49cd6bccf7be318997acc79745250a`  
		Last Modified: Sun, 02 Feb 2020 10:35:59 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1719f3ca6300f86e468242312c23adbde13edfb69da566acdb515d67e0285e58`  
		Last Modified: Sun, 02 Feb 2020 10:35:58 GMT  
		Size: 1.3 MB (1309493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12068913b9eadd4758fa283755c0081c35274d2d7b304257b3c8d3ecdc1dfcf3`  
		Last Modified: Sun, 02 Feb 2020 10:36:00 GMT  
		Size: 8.0 MB (7965114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a862a006e9d757167d50e3cdd87bff07997c60a8947751f7dce5764eb1c67b`  
		Last Modified: Sun, 02 Feb 2020 10:35:56 GMT  
		Size: 297.1 KB (297108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d204e55de65af43d3a5f2f4a58cb2967c012da696881f6598b097b8278d9f7`  
		Last Modified: Sun, 02 Feb 2020 10:35:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14994cf874f0aa45e27c3b9a97fdda202f094757880776a3295db75e4f8816a`  
		Last Modified: Sun, 02 Feb 2020 10:35:57 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1044ab3ecec33f97178aaf48e7315a37260d993e339fbe9918e68d0d1d9d793`  
		Last Modified: Sun, 02 Feb 2020 10:36:26 GMT  
		Size: 86.2 MB (86164394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6bb03ce7e1ff28a09268597b0d61d54f7a7f746e76e357b0819b0e6804fbd2`  
		Last Modified: Sun, 02 Feb 2020 10:35:54 GMT  
		Size: 8.9 KB (8939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dd490aee024ce23ca9ea1dab4fc770e1f20ffcaace82da79c98588ce10df6f`  
		Last Modified: Sun, 02 Feb 2020 10:35:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb67c8e5cb7606aa7f42b2e41ad8b1a6cf1194fd356447ea134d9c170f3c1e61`  
		Last Modified: Sun, 02 Feb 2020 10:35:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1182cce53f53d63a2af207b18aa6a8cd3471fa6791f310cdd5817d1849942e4`  
		Last Modified: Sun, 02 Feb 2020 10:35:54 GMT  
		Size: 3.8 KB (3832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb577abd486e9dbfc5d60bf46877ea34722caf1da72fc776927c2bfdc4c7444`  
		Last Modified: Sun, 02 Feb 2020 10:35:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:84e698fb4afa52b26cde4a2051a59c82588bea38db83482cc3f8a4f7ee80b618
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128797621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3303d3b3ff18b18cd346da028b5c910bfd08f33ed9853b6d4e174faa5134768d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:55:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 01:55:56 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 01:55:57 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 01:56:19 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 01:56:34 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 01:56:35 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 01:56:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:56:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 01:57:00 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 01:57:01 GMT
ENV PG_MAJOR=12
# Sun, 02 Feb 2020 01:57:02 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sun, 02 Feb 2020 02:23:05 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 02:23:10 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 02:23:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 02:23:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sun, 02 Feb 2020 02:23:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 02:23:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 02:23:17 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 02:23:19 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 02:23:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 02:23:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 02:23:27 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 02:23:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f388bb0aa851f4bf41a6d4990a5b02f92e8dec9fb0a4bfb1ad69670c0499b56`  
		Last Modified: Sun, 02 Feb 2020 04:06:47 GMT  
		Size: 4.2 MB (4170031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfd56988f6c52fdcd2d9364dd5f02671bd03dca661e9cd79cb84e440d47f49c`  
		Last Modified: Sun, 02 Feb 2020 04:06:47 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a40467cb81173237a90ca7fd832b2f640fcc61df67de14b116d11155f21e6a`  
		Last Modified: Sun, 02 Feb 2020 04:06:46 GMT  
		Size: 1.3 MB (1292567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127f0bf8802acf134c98076466679b64c6e65cbf3b3bf84e6f5c7b7620e4906b`  
		Last Modified: Sun, 02 Feb 2020 04:06:47 GMT  
		Size: 8.0 MB (7965115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12f0ff25dd163f3615a82239240a6147716e292cebfa708b9df83d46c92b718`  
		Last Modified: Sun, 02 Feb 2020 04:06:44 GMT  
		Size: 297.2 KB (297199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baffb02ad63e236b4b1a60fe916f3283fdbcacc3c2fbe380b53af2dccd712429`  
		Last Modified: Sun, 02 Feb 2020 04:06:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cc9d652d0a38de69666934953e5af2321eb0f6a84afe690b94eb036738fd28`  
		Last Modified: Sun, 02 Feb 2020 04:06:44 GMT  
		Size: 3.1 KB (3051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c0f8af1fb17cc42a7066ea764d4747916604e67800c9acc53483c4396a429e`  
		Last Modified: Sun, 02 Feb 2020 04:07:09 GMT  
		Size: 89.2 MB (89203814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bcf88097d6a9a863d486a53f101e3a8a8a8079960a6eea1277c71e9068d4ef`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 8.9 KB (8945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e40f39b0845fc6dcec06ee81dc497da1637af40f8ae2581d38f218575c4522`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e82f218dc48db49d1cf10b85b8315ebe6d7545238b2d461c6109df8f197bf3`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae8120259ba3b59c5a6cae2887712e0bf2edd6a38b3703a6698417d22251353`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 3.8 KB (3832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13a9fbbe5768e499a5f52e3fc7141ebd64f3cf00682fc621ae6eeef194dd7c3`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; 386

```console
$ docker pull postgres@sha256:15d2b662bf217b36a736f1d02def3998ad6fa9ccf4437443248dac4c7c6cba75
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133605313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:646513813d7977878d6723e3ae2482e4272085c4a7e6562428133c14aa19cf05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:19:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:19:38 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:19:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:19:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:19:58 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:19:58 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:20:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:20:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:20:06 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:20:06 GMT
ENV PG_MAJOR=12
# Sat, 01 Feb 2020 21:20:06 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sat, 01 Feb 2020 21:20:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:20:40 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:20:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:20:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 01 Feb 2020 21:20:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:20:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:20:42 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:20:43 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:20:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:20:44 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:20:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9997cc045ec61684d5eec173034939f749331c09514c0f8f613d25d901dc1024`  
		Last Modified: Sat, 01 Feb 2020 21:26:55 GMT  
		Size: 4.5 MB (4542204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66be524cdc140df03dbcccd1a976d544f2e4829fc9bfc3e7bdccc89599795d6`  
		Last Modified: Sat, 01 Feb 2020 21:26:53 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398bfc0869d06d06235249409f9b9f5e47c7ce448f9d463d9a2cd70f0880bfc`  
		Last Modified: Sat, 01 Feb 2020 21:26:53 GMT  
		Size: 1.3 MB (1324297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655574080d822c8be4e7c5cae573ea8f54a9253cb9c1832c1f6a410992cc1ac9`  
		Last Modified: Sat, 01 Feb 2020 21:26:56 GMT  
		Size: 8.0 MB (7964334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855eb32a60e3afa4f766aa8d5c7bcf756848c25bad82dacab8e4c1b194a62c64`  
		Last Modified: Sat, 01 Feb 2020 21:26:52 GMT  
		Size: 302.6 KB (302646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a231a2303f474ca777cfd033c48642e0697ef96ae78a91b7b1c8c06efa2adf`  
		Last Modified: Sat, 01 Feb 2020 21:26:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4d191a2ed807914eb97dedc8af739d87405c38a5cfe6253ef03b94e55f8466`  
		Last Modified: Sat, 01 Feb 2020 21:26:52 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bef7e7e0ebb599b2a52cbbcf6bba8d0abb411477c3e8929b6a8893259d049`  
		Last Modified: Sat, 01 Feb 2020 21:27:23 GMT  
		Size: 91.7 MB (91706653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416302b0bdc10382b71f0422598b309abcb0431d26a98bf11af535d507ddf148`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 8.9 KB (8939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01dd73843a8b777c3d04e4d985aeed22fb46c77680776bd824fe84ca758284a`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26acb787c93edcdaad18e008fb60074aea01398dd3c30de4a95edf9f0c92e76`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278773a18c87177bdf3a45a07849805beba861ad6b22d2955f3ce51c6d4c40de`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6d274516a60cf901e0dd529b59c13ed19cc956416fb0083500adee1cae5d5e`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; ppc64le

```console
$ docker pull postgres@sha256:215dc5d6669a1da21d5b3085c2c7c9f38535f79d1623bcaa1abfc4b11037703f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.7 MB (140661747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ea846050bcc433b0a867bdae9ea6aff85550d9cb39c9fd19babe6daa05d55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:04 GMT
ADD file:aadd94011800934ec665edb193029ab2be0aeb668c566ba4bc52bd678e71a735 in / 
# Sat, 01 Feb 2020 17:18:06 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:28:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 22:28:51 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 22:28:55 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 22:29:39 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 22:30:02 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 22:30:05 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 22:30:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:30:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 22:30:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:30:39 GMT
ENV PG_MAJOR=12
# Sat, 01 Feb 2020 22:30:42 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sat, 01 Feb 2020 22:33:08 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:33:19 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:33:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:33:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 01 Feb 2020 22:33:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:33:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:33:38 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:33:39 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:33:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:33:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:33:49 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:33:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:16a7e1c5b23ec3cf93421f5f868c1cf2cda468cfebb1b2bc62f4d533d99d256b`  
		Last Modified: Sat, 01 Feb 2020 17:26:05 GMT  
		Size: 30.5 MB (30517693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4887b42e3fa4bab4b6a923a23616405501ac3a66a9980379276a018032fcba51`  
		Last Modified: Sat, 01 Feb 2020 22:57:21 GMT  
		Size: 5.0 MB (4967152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27430705fd8e84fe0517512f555ef1ba8cc7a678cb11ec355b1cb20c6fc5a86a`  
		Last Modified: Sat, 01 Feb 2020 22:57:17 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dfdcc823e3bdc8b3c097c0692c8d7e18bac53a5c81d492ab4a0459851d8f1d`  
		Last Modified: Sat, 01 Feb 2020 22:57:16 GMT  
		Size: 1.3 MB (1281132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec861509b6b231e57138dbd3e70c457a6e9a37723dab364034f3db3132efdeb`  
		Last Modified: Sat, 01 Feb 2020 22:57:17 GMT  
		Size: 8.0 MB (7965285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8d1e2714f7c11d0d4f86e45f6b4c185ab5415036ce792cc5458b1f7d2d040f`  
		Last Modified: Sat, 01 Feb 2020 22:57:13 GMT  
		Size: 298.4 KB (298419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace9017f0ac376a5945ff5e4539ed18191f8a3ed9393442110a476621cc0e02a`  
		Last Modified: Sat, 01 Feb 2020 22:57:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4835b320e4b6d061c58f94a862d753376ee1cb29e6121a43896fd5a14aafb8`  
		Last Modified: Sat, 01 Feb 2020 22:57:11 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745126f068ad315829ea29cbf2653902b92bee847d70eb57f54bc98f8f8fbc11`  
		Last Modified: Sat, 01 Feb 2020 22:57:35 GMT  
		Size: 95.6 MB (95613824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64bea14266964a29c5e52db3dc270408dc11e05737b1984557ebd3a681d662e`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 8.9 KB (8946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67701b86081c69f032a3e349694d7fae90ab23601989775860189405fc7e0f4`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0f69553453dbae98a758499e7f56e80bcb8c2f5974e75e19bc0dedeb4173c0`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e22e6b585a6acc8c623bcc1df9162d64414d3e450c536420781a505eb317e51`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d1338c638f8b6969a45c4e701eae1e7fe15b618b7b2d6b3f81923114c1d439`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; s390x

```console
$ docker pull postgres@sha256:fd2eeeccb8821e23ef204c28a973d77bb9f8df17f2ffecf013902e072cd242a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130699858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4c8412c11232f198d75c5bda5db095c94996b1e967df11d477642f88e37d09f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:31:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:31:16 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:31:16 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:31:27 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:31:32 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:31:33 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:31:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:31:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:31:38 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:31:38 GMT
ENV PG_MAJOR=12
# Sat, 01 Feb 2020 21:31:38 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sat, 01 Feb 2020 21:39:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:39:44 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:39:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:39:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 01 Feb 2020 21:39:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:39:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:39:45 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:39:46 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:39:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:39:47 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:39:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74fefbeeb6df5424be490954827987a8c7927e23533e2b454167f45022c7af5`  
		Last Modified: Sat, 01 Feb 2020 22:14:51 GMT  
		Size: 4.1 MB (4059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895f0676ff0f3afd82aec3a77b255c9c0c581b5e803f23827986d19fc5f6f50a`  
		Last Modified: Sat, 01 Feb 2020 22:14:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e654e4a94e69c38789dc3333f9302ae6da13fd5ad94357b844ac9ca012bc21e`  
		Last Modified: Sat, 01 Feb 2020 22:14:49 GMT  
		Size: 1.3 MB (1347168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85405aa2bd96afbcab08a204fb2728b768360ce8825d8a11b53b859cdc28076a`  
		Last Modified: Sat, 01 Feb 2020 22:14:50 GMT  
		Size: 8.0 MB (8019246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a965d11c59c3785fdb3ffab95e8098799bc345f0d290afccacaf7062100d5b`  
		Last Modified: Sat, 01 Feb 2020 22:14:47 GMT  
		Size: 299.5 KB (299520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6431faedce67353c59a7a1f079a4562b05844dc6695c00abf4e0eb3d5b27e`  
		Last Modified: Sat, 01 Feb 2020 22:14:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eee97bd06c29e84244a7eab8914aa3778a4e89a8624ad8f965739a260dd35d4`  
		Last Modified: Sat, 01 Feb 2020 22:14:48 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e608d8ade99e94ba7d5615dcdf94f6a2f1df41bdece8d052a8dc8e99704587`  
		Last Modified: Sat, 01 Feb 2020 22:15:01 GMT  
		Size: 91.3 MB (91250606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76288b6b5963a068ab28c11a4c31b8bcdb74553d6d61099a513ba7f8ec6d71c`  
		Last Modified: Sat, 01 Feb 2020 22:14:46 GMT  
		Size: 8.9 KB (8943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80abcd2ec4ac20a6cddc78ea6bc2b361b62ecc324287f3b01493fac33c890361`  
		Last Modified: Sat, 01 Feb 2020 22:14:46 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7973374d8873226e1a70e8b705ef61c6a1dfef5bdd5254c521ab4df02b372013`  
		Last Modified: Sat, 01 Feb 2020 22:14:46 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0bff87841570aa5384d2c2f7e95d968007d37842dd2d58798cc450ed1e997d`  
		Last Modified: Sat, 01 Feb 2020 22:15:01 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ee830e8ce7dd8e5796449373587307b40da2a6d372f7a6745d95aa7f83887`  
		Last Modified: Sat, 01 Feb 2020 22:14:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:12.2`

**does not exist** (yet?)

## `postgres:12.2-alpine`

**does not exist** (yet?)

## `postgres:12-alpine`

```console
$ docker pull postgres@sha256:686fc517b2b979f972aa2cdbdb4e3392f28b7d6e6dc31054c05144863e6d9098
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:12-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:6d1510dc1fb520e346b9e653c77941ab3ad8db1081b519296dcfabfcf864d393
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60209239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76780864f8deb0b48cdde6aab3069e0735f5c19724a287d91ae7f448831a54e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:19:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:19:59 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:20:00 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 03:20:00 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 03:20:00 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 03:25:23 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:25:24 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:25:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:25:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:25:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:25:25 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:25:26 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:25:26 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:25:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1030c456d04636112fa347ddc5296036cddf70c8085be2e3f3fb481898f18fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d0211bbd9a4fd28f739a797600d78394b15d947a30f55f70cfd5daf0f9e443`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8060dfd57b68c41186b9460b303cc45b5e4d68bc8a0068700dec4f1bb0f47b`  
		Last Modified: Thu, 30 Jan 2020 03:43:04 GMT  
		Size: 57.4 MB (57392577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0905212eea51fe66acc2cd9fef63f91d73ffe7dfa3b27311ec4ec393b8fad2fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 8.2 KB (8211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a126b91cf92ff8940d9f65535c747079fee16d71c27618142eca0bac7ebebf5`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45f87d751e97454b063f18ded1bc280660fc1c616affdc0dc2210e9e805d446`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2148a93fc26ec6eb896ae6b4e0470106722e10feef81cbb83e6e8fe3459b4ec9`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:e4109cdc27e39a043b52c2eeaa5ebccaec6c8dbe9929ec0e5b493cb6b391f459
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58622281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea62dec9853c1679984035cb61af6d5e93611140410ffb1967f8730b35850cd3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:49:35 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:49:36 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:49:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:49:38 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 02:49:38 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 02:49:39 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 02:54:02 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:54:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:54:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:54:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:54:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:54:11 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:54:11 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:54:13 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:54:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab27e2422be886bc0a338b0e0c20b8e2beea15b880defbac81f75c04495d0c2`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae2520a8d4cdac962b6d4a62335dce896f8ccb0b6d2693b0e72591fda026d14`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a722cf47a5d9e2ecdbca0527baed31e0c969df84292cf7b4d535fb1ed008c1b`  
		Last Modified: Thu, 30 Jan 2020 03:12:06 GMT  
		Size: 56.0 MB (55990889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fabaa46778b33fd058aa9ad21f3a88457aa6a4bc2a7711c946041fdc5683b6`  
		Last Modified: Thu, 30 Jan 2020 03:11:48 GMT  
		Size: 8.2 KB (8212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2e893a8b4b319a0df20d5548433fdd1a8aa768ab6c43243613958c68b83a1`  
		Last Modified: Thu, 30 Jan 2020 03:11:48 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045aee12c861e00b0238d8fa98b0d9858380be6b06f99fa6b73132c5f8ccc384`  
		Last Modified: Thu, 30 Jan 2020 03:11:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25638010d03799556d44805f65a28ec0b551ba92c81e3ef6b0d758690bc1a44e`  
		Last Modified: Thu, 30 Jan 2020 03:11:48 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:490812945c2aafee90a8f4f030c79c1ac126eb3f2fdf1a49d9f36d77b0fae8ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55877719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff0f3c5a5f64747e220a0e46108b50a759ed99c694655c0779c8737815fbfa0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:00:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:00:13 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:00:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:00:15 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 03:00:16 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 03:00:16 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 03:03:18 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:03:27 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:03:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:03:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:03:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:03:43 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:03:44 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:03:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:03:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572777a7d0992ea05b14f2ba3230ce906c753dd21eb73ac2b6018551250312db`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8810228251d658112d3dbf2b9b1719f402a0c3477bf2eceaa5a20341bba3f5`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0440024149898999f2925fad16d0906a5acaf582f137c092e6ffe492fba0050c`  
		Last Modified: Thu, 30 Jan 2020 03:18:53 GMT  
		Size: 53.4 MB (53444337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0b69a13b1e0d55e13b022cff4762658c1c132e7e09b8ee2c7abcd37a64731f`  
		Last Modified: Thu, 30 Jan 2020 03:18:33 GMT  
		Size: 8.2 KB (8213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d27ef35e1dd04911e24e1661facbedf0553fc74a1a30164404054b21070af51`  
		Last Modified: Thu, 30 Jan 2020 03:18:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4fb7b2447189f17d739416e48d823db0c6265efbd462c3b08af30f0127fec`  
		Last Modified: Thu, 30 Jan 2020 03:18:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8487f1ad10109177a9830bea21caf784094c75a928a54f20ffda4aa42081f7d`  
		Last Modified: Thu, 30 Jan 2020 03:18:33 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:50229cfdcf2f0e58017cbfee317b7d9f77dcba8adef0fc77d8cf075c146f72ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.8 MB (59816718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79852caddd0e2d71f36f8f8f7d04fcc9dfb82942f42a2f960e8cb8cff2b9fe4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:40:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:40:28 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:40:30 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 02:40:30 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 02:40:31 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 02:43:37 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:43:40 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:43:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:43:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:43:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:43:44 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:43:45 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:43:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:43:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db837ff5778a13ace9e439e3bff33c317ecca84803a142a4ee4e05d2af54def`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92b445ab1ef4ba9a6120e5cc359b70cb88b74a46dee803f2709cb873a7be79`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc686d41f5bda50e8af88ab466c917d3719483d6e6cce75d4320d1f8e3a31ad`  
		Last Modified: Thu, 30 Jan 2020 03:00:04 GMT  
		Size: 57.1 MB (57079817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040995314274c90b4219ea0616a0fe8f55de7a69c460aa81f9d1e0842855591f`  
		Last Modified: Thu, 30 Jan 2020 02:59:47 GMT  
		Size: 8.2 KB (8211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2cb564210a010901427bc0ecc92a3c74aebe110023a4ac458573f844d68e11`  
		Last Modified: Thu, 30 Jan 2020 02:59:47 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a7e8cd95fdb8cb6e9e8e2eb11de181f434cba8ea5ed233f734c718ba17778f`  
		Last Modified: Thu, 30 Jan 2020 02:59:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c6872e0ae787aafd709d552a37c873e9aceeef6f134b7ca83fe97b33bea5c7`  
		Last Modified: Thu, 30 Jan 2020 02:59:47 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; 386

```console
$ docker pull postgres@sha256:2707fdc5fc7de80d491a50742a9c4d452880a6baccee46626165aa93ee2504c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63503075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a283ed7bc47149212e65b1e1b48ced1b0cd43db32bb395784d54916e84c43c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:38:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:38:44 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:38:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:38:45 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 02:38:45 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 02:38:45 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 02:45:21 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:45:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:45:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:45:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:45:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:45:24 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:45:24 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:45:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:45:25 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:45:25 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb8463eb063fd24e3d29bd4ca5b9ba1590717acda7415cb45da3e7560f0dd`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023c33adbfeb9b779f40edac1617b4514e1fb0b976b5b201dd0f7dc688f5e60`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12d7f06890c46cd61cdaa35d77c6620b9f7bd0e18f56ab12c7223573682c6e4`  
		Last Modified: Thu, 30 Jan 2020 03:07:33 GMT  
		Size: 60.7 MB (60682813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717eab95de5727f2647df81a3e623422d0d6da0f1a239f81f49beb29da19ed08`  
		Last Modified: Thu, 30 Jan 2020 03:07:20 GMT  
		Size: 8.2 KB (8212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8645372b3f8e19172b59c419fa904284db7569a7244dce048f107313a738098`  
		Last Modified: Thu, 30 Jan 2020 03:07:20 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74908cfa3379c7f9699b55c2f166404ea9145f670dfeb1ae9907f4eb422faa88`  
		Last Modified: Thu, 30 Jan 2020 03:07:20 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a2aa22249caa908445eff022e57e64ec35416b9c0813ad87742b6905026bea`  
		Last Modified: Thu, 30 Jan 2020 03:07:20 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:0509f725b358344ddf92d48bdb36beaae366f0cf392d9d320380889e40c36ef8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62508393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec010b745eb40c664b023633d12d09ba4adf7c8a449a0b62dad251eb59f21d6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:20:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:20:03 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:20:09 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 03:20:11 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 03:20:14 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 03:28:11 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:28:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:28:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:28:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:28:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:28:47 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:28:48 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:28:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:28:52 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:28:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8af198a4c612619984a3d16dc2a9fb3f15835dfbf5269a9eab9a345ed4f14`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852af7c4759ead6b82b170b6d34d124532026b41ec5d7dc4ec99bd6705f633a`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968c03fdd050acad3b1036cc889688f376662a89a0e9377d86e585d3bec6e560`  
		Last Modified: Thu, 30 Jan 2020 03:53:37 GMT  
		Size: 59.7 MB (59672450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8270fe06fad89a92a1fcf843edb82f944e375302ce0a8645a769254afc6d12e`  
		Last Modified: Thu, 30 Jan 2020 03:53:23 GMT  
		Size: 8.2 KB (8205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b07968249434b685ebe4e9e31641af2993e2561ee3dd9de65086e82b85a1a6e`  
		Last Modified: Thu, 30 Jan 2020 03:53:23 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85aadd28933545b5713d7bba52777b3aae9f2cf1d6b72c031c0ab5abf34be6c`  
		Last Modified: Thu, 30 Jan 2020 03:53:24 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b1103f24667299f066a0e1d773d9e65ef0a85987c1f834be8534a9d7937659`  
		Last Modified: Thu, 30 Jan 2020 03:53:23 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:4d0a554cff31942375880976aadb1bc9258873c3981187d00485d90e02e5f9a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62394435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f13f23ba24a8992c41390967d4fc5914ff22783fa9dd87a36934f29f906afaa2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:48:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:48:56 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:48:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:48:56 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 02:48:57 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 02:48:57 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 02:52:48 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:52:51 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:52:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:52:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:52:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:52:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:52:53 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:52:53 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:52:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d0ab56996305262d42136eee090848bbdf7cec28b8625e39078668b245db48`  
		Last Modified: Thu, 30 Jan 2020 03:07:31 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd3ab8f7e8df3f56e9628a504d2ea6db996a9910565bf84e3bc35bd847bcfb`  
		Last Modified: Thu, 30 Jan 2020 03:07:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86991534af0dcfa73489dd57b1a295bc670d98a42a40efdfbf572f8d95ea269`  
		Last Modified: Thu, 30 Jan 2020 03:07:35 GMT  
		Size: 59.8 MB (59798579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fee2b3b6229935dc8ac2f31f799d5edf0262cd79292f61e84f4ed7aa3a882a`  
		Last Modified: Thu, 30 Jan 2020 03:07:43 GMT  
		Size: 8.2 KB (8209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692fa998ff3b5325e278680c19ae2154bb46299aa4be960e3c9fa9eeb9543a7d`  
		Last Modified: Thu, 30 Jan 2020 03:07:43 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa365558bb0a4cc0bb7369a209c91a15d37b4dfa15dd986008e7ac11382ac2ea`  
		Last Modified: Thu, 30 Jan 2020 03:07:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b6155a6baaee4d9751e478b81242eb8d4b081df17ab10044012445ff8daa7`  
		Last Modified: Thu, 30 Jan 2020 03:07:43 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9`

```console
$ docker pull postgres@sha256:d6a6badb2b5b22de5e135490a217522cecc2ae90fe35b33290615827569310a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:9` - linux; amd64

```console
$ docker pull postgres@sha256:c5df9349b2a361769ea3859d9d6b675cc3c08aab564115ab936632447aed15be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87992167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb2889ab0680ba518e0dc1bb5a09cbe23f1e5908d9e484daea3d34f5e092ec17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 06:07:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 06:07:31 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 06:07:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 06:07:59 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 06:08:00 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 06:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:08:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 06:08:12 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 06:09:45 GMT
ENV PG_MAJOR=9.6
# Sun, 02 Feb 2020 06:09:45 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sun, 02 Feb 2020 06:10:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 06:10:10 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 06:10:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 06:10:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sun, 02 Feb 2020 06:10:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 06:10:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 06:10:13 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 06:10:13 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:10:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 06:10:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:10:14 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 06:10:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0fe6664f6bb5f06d5d0a9a68c99a68be052403c684a8ffd98e70f6256d8ca`  
		Last Modified: Sun, 02 Feb 2020 06:12:59 GMT  
		Size: 4.5 MB (4501301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7ba8f77640450af762ebf643f368663949425d1bd516521dd9c0022a65461`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 1.8 KB (1779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1155d037e2c8553fc58b2671c2e61ca9ee29c7f712dbfc66dc20e8ab549c6b`  
		Last Modified: Sun, 02 Feb 2020 06:12:58 GMT  
		Size: 1.4 MB (1351457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febcfb7f8870017ab69faa0a454aa6a1e3cfde53c46074d1aa3e6edaea01adcc`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 6.2 MB (6182941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c78c79412b5cb255309e404e829646cc509a10cf8f55b2a5043da04d706604c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 295.6 KB (295582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a35744405c5f473d3002c5451970e6ff78bcc5eb330eea1c5595cca6b32679e`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27717922e0679badf783f2aa3179d254bb023533caf48d859c3d29723401701c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577de7c4ffdc4243fbaee8f228488837f2f9a2f2c87a68202abaea93ded28b88`  
		Last Modified: Sun, 02 Feb 2020 06:14:00 GMT  
		Size: 53.1 MB (53117400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3482e27d98ae9056b29a5cdd582dadcb8ca915fcd335fb73b061a85e50b6f8`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 7.8 KB (7823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ff898274ac109dcef4fcfa92b07409953f2f4363ecd0d73cc0b004f00f0815`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6131782ee224b1daac69e6d7f6b38b744422334fb5906b6432e929c3d32782`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496ebd477eeafd1b47febb4fc082afafd21079521d1b93c519265d5bcbe0e414`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f0da1de185b12370cf4623340f2058fa5a2a3560fd926d0e8b07f6fa22cb30`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; arm variant v5

```console
$ docker pull postgres@sha256:156b34423cbba4d94ba6cdad7d3f45648230879051597dca3222c8a8f87c0245
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84491279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9103688e54d3b96fec8326d286a3bb0a3680ab194f4a7ec614c89051b989eb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:53:57 GMT
ADD file:f0d179649cbf50028b5ecd832961cc332fb524c2f12fda6c8060c3c258208be6 in / 
# Sat, 01 Feb 2020 16:53:59 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:04:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 19:04:31 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 19:05:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 19:05:16 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 19:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 19:05:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 19:49:02 GMT
ENV PG_MAJOR=9.6
# Sat, 01 Feb 2020 19:49:02 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sat, 01 Feb 2020 20:09:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 20:09:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 20:09:20 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 20:09:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sat, 01 Feb 2020 20:09:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 20:09:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 20:09:27 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 20:09:28 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 20:09:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 20:09:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 20:09:32 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 20:09:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:03886a8604d1b5423798ee97917dcb9de4cfdfbb7c435a7988d5c5e69a78e3b7`  
		Last Modified: Sat, 01 Feb 2020 17:01:03 GMT  
		Size: 21.2 MB (21202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aaa01ea1502b56b5ebd804228ff2ea5ad2adf78d4797d7a6aa75903a7dc7a30`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 4.2 MB (4236888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feeb9ed754ebd60d2d8cdffa636ff7e5b6ea1b1f68fd7c7aac5f1dced2f8cf9`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142683156b4ad1e2209ecaac30f55cd1a7237fe046f545e7a64613b34c221671`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.3 MB (1311293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950d1d965477d4d1230281bd3043f7347d94e263cada82cd86f3f055cc269e93`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 6.2 MB (6185421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1690d5dc7daff0def912cfa3c22eff87c80edb8f734454280c116e5fd52ebb92`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 293.5 KB (293479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0191375b3084722e33f875137d737673fc3ec09776716614c4fcd6764e7884e`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9bf11db5cc7dd3ff01824ff16d5642657294a22e3ec2086a5b3575ef803947`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 4.8 KB (4791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0243666d93d53a13ddedd28e800d1c27f6d6a89faabb40345177bec3ad01664b`  
		Last Modified: Sat, 01 Feb 2020 20:52:15 GMT  
		Size: 51.2 MB (51242498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a8b7d0740023a25af9ac759b731a38892cd1b4944e18d5790549e52203ee4e`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 7.8 KB (7822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d17cd9d8d74696e07f0eb85d3232d957faf2db274d18f0d7c53043b786834`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724495e2c1ced93f7ae7635b5653dd7d82256e8726814b76e32668732e9a2432`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fa4ca3b32534986ebdb3e5a073f4478ed6e34bec824033f13822a3313dd03c`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5708c0cab5dc7637b4e00100d14dc31ef6438188a0d43fdadfb1cda8e9b49087`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; arm variant v7

```console
$ docker pull postgres@sha256:6176db12c5cd603cf2deeb0ece0c394a94a0b491f5b34418adf90bb2959118bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80638829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df1d2a74bab23c4cc256ff5e5f7a91965712471e65e31155b72fe23970346cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 08:58:06 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 08:58:07 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 08:58:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 08:58:44 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 08:58:45 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 08:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:58:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 08:59:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 09:40:04 GMT
ENV PG_MAJOR=9.6
# Sun, 02 Feb 2020 09:40:05 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sun, 02 Feb 2020 09:59:01 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 09:59:08 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 09:59:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 09:59:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sun, 02 Feb 2020 09:59:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 09:59:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 09:59:17 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 09:59:18 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:59:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 09:59:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:59:23 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 09:59:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e359f7642afed089b2d05ece4e0736e03ceb13a937f7478eb868702665f809`  
		Last Modified: Sun, 02 Feb 2020 10:36:41 GMT  
		Size: 3.9 MB (3872826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b5742cb7fbb2cdb38f99c354efd420d24d27dee9b21b232dc92100066c10b`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6852094413bd98c461152c87837e91176b94a6cadae25e1a31b7f07330ecc4`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.3 MB (1303620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589bd77312350a872d2ebc5a6638ec844bf3aece0160a35b34a5d5cf66ae0d22`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 6.2 MB (6185708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943e832035ee98c3689f148b48e73550099b8f81fe37da09aa6e1ae2ea1756ac`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 291.9 KB (291867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba8ac21d907e788e2f05af094077cd10bcd20b8bb6eb5021b9f01ae1cfb1d97`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f8d5c6112a73a87453a9f3b2c2c298c0d2c275026fb63fb5ecdd81e6205461`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 4.8 KB (4792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ea67ee1c6fb5d3075dbf0b963e7d7689e2393a836c4a3b3065195103a393c3`  
		Last Modified: Sun, 02 Feb 2020 10:37:51 GMT  
		Size: 49.7 MB (49654325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc7ea1bf1b3ba1ffea659c5edb02dc3dc37ca858be0093a87bb3098bb6e6315`  
		Last Modified: Sun, 02 Feb 2020 10:37:31 GMT  
		Size: 7.8 KB (7819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1591631eb0d69c23e4d2116eeadb0aec1ae49bbf686e3c1cc9829847b19cc5e5`  
		Last Modified: Sun, 02 Feb 2020 10:37:31 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e59bda490195f44526b0ff46921e8c3216469ee27448053793917ecaf4561df`  
		Last Modified: Sun, 02 Feb 2020 10:37:31 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd73775a0650bd8db6494735b191ee5b9a411883de6a7e25058138a7af0ca60`  
		Last Modified: Sun, 02 Feb 2020 10:37:31 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd23b1945cdfbfdc79db97f4aa956fd8f7ba1affe7121cb367da74b4bf8ae3`  
		Last Modified: Sun, 02 Feb 2020 10:37:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:3fbc177c71c33002547b77433ed04c2f54964c582ea43ef9d25c4edb94d87366
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83499997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9706bc1df961358808bfd77c775181ec51651ad54e6cb57fc25f9b6381ad04a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:24:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 02:24:24 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 02:24:27 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 02:24:52 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 02:25:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 02:25:09 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 02:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:25:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 02:25:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 03:08:47 GMT
ENV PG_MAJOR=9.6
# Sun, 02 Feb 2020 03:08:48 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sun, 02 Feb 2020 03:28:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 03:28:27 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 03:28:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 03:28:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sun, 02 Feb 2020 03:28:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 03:28:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 03:28:35 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 03:28:36 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 03:28:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 03:28:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:28:42 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 03:28:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a29899232ff5984832260695109c206ed14783ab8a33dd8f593f40672e2cf51`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 4.1 MB (4077687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72390476b7ab26db4e6e224ad16f9c0a3d66dce6b4d9996f6edece0992dec78e`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4470eb370695bb8691186ee389e7be5deaeb4f0d84a84ca948ae39ea977a1`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.3 MB (1286440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b51db6dc34b50eff6b5d8120f3efff4e5269216d5ea5d004ce80782e7508411`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 6.2 MB (6185392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918217c35d15c52bb58861e8c65a6b6934bc554387043c67b630758273c41028`  
		Last Modified: Sun, 02 Feb 2020 04:07:20 GMT  
		Size: 292.1 KB (292139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea01905f4f686b651e994714cb840779b241fcf43c04c6cc2a0ae229543862dc`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ff0687a25d7e24b75be4e353f57d8821a81a4b8c51aff2a01f927bb70d1a76`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 4.8 KB (4794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424f08e065d6d18e3d2b4ce50ddede234d07b7cd7f54aa614eb5d92a1862ce8`  
		Last Modified: Sun, 02 Feb 2020 04:08:28 GMT  
		Size: 51.3 MB (51253618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b912d4a038fb1bbb67af442be67dd04e068043b1f07167149b5dc1bab352b9`  
		Last Modified: Sun, 02 Feb 2020 04:08:09 GMT  
		Size: 7.8 KB (7819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2539c3f1d8eef8f0f55c2471f0896f3e7448e6fefea11731b315999ab35dee`  
		Last Modified: Sun, 02 Feb 2020 04:08:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02a4185c7f2fe75b83ce98818c61040b6066de3db6eabcb5dc3c56d80ea411`  
		Last Modified: Sun, 02 Feb 2020 04:08:09 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae02c764537af80292160bf0c69b4137d6163ccea411bd4ce93f4dc0e10790b`  
		Last Modified: Sun, 02 Feb 2020 04:08:09 GMT  
		Size: 3.8 KB (3848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94f68ec254f3c01c9811f77eab5b38bcbc19f18cdb79a16bc9dde24b20d71dd`  
		Last Modified: Sun, 02 Feb 2020 04:08:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; 386

```console
$ docker pull postgres@sha256:0cc60c7ca6aa2b656d5be080630da5245a1d25547e5d531580ce826d789e165d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89369641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b07066394842fba9794666320ff1073131f9849b1e76bb494969683718fa1b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:21:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:21:11 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:21:27 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:21:39 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:21:39 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:21:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:21:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:21:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:24:05 GMT
ENV PG_MAJOR=9.6
# Sat, 01 Feb 2020 21:24:06 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sat, 01 Feb 2020 21:24:47 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:24:49 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:24:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:24:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sat, 01 Feb 2020 21:24:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:24:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:24:52 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:24:53 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:24:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:24:55 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:24:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400715a0cf80a4163f9bdfb01029e10c149b8ff3ce6ef1248f400451f617b081`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 4.8 MB (4807817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57223b59a38681596adf27043fcaa0c4896293e4b8d488d81957c76d11ee0d7`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb13941b5f12a8251a7c85981cb0d44069be9f4d1644bc34a11ae761968abdd8`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.3 MB (1318016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ada6bc6e6f24824fc92e6f96abb0ec680d29443a640d4b03d2ac54a6cb74ba`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 6.2 MB (6182955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65761eaa1a3239dc440a674c9a27612170189ab04f41d5360678cc34ddfab827`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 296.8 KB (296752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81305139d5a6d74e0ed5bf9ba0163f5c6baf0c66890f74d05e94b5313a57d86e`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ff425a04fcdc853777162926c616c569257ea00e96154204e9e3f91e2f7527`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa669fa7d13b33dbd17a9edc07645f1d8055817b4fca8ab2ce671f36d9c9fca8`  
		Last Modified: Sat, 01 Feb 2020 21:29:09 GMT  
		Size: 53.6 MB (53593187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018e1562dfbad2ab7b61a76e7ba8fae2df8289ec6bfefc5f33b450c6a382bea5`  
		Last Modified: Sat, 01 Feb 2020 21:28:45 GMT  
		Size: 7.8 KB (7817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a85f32c119e7b1840ce73e2514c57b808d291dbb573a8e25bf5e8272f7669d`  
		Last Modified: Sat, 01 Feb 2020 21:28:45 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36872fb92973a9d1aef694535a04ea9e87f661d5e378927dc6c3b4922f790c8`  
		Last Modified: Sat, 01 Feb 2020 21:28:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e02424a08286578a82a1c2ca3e657020c6d852022f3c62a2a705dc9ba91f60b`  
		Last Modified: Sat, 01 Feb 2020 21:28:44 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82941b4e2b391ceb761d3d6f6d27b8569dc2a9ee4a35a24c0cf62c085eaeaaa`  
		Last Modified: Sat, 01 Feb 2020 21:28:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; ppc64le

```console
$ docker pull postgres@sha256:78828c61f1b443c1ada7ffaf07ccd43d6cbcc1ab539d2e27862920106ec4b856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87711767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6f614dda0c03db1138211867f66644c057e66e8171997d60481600b17119483`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:34:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 22:34:47 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 22:34:48 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 22:35:35 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 22:35:55 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 22:35:58 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 22:36:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:36:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 22:36:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:45:00 GMT
ENV PG_MAJOR=9.6
# Sat, 01 Feb 2020 22:45:02 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sat, 01 Feb 2020 22:47:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:47:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:48:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:48:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sat, 01 Feb 2020 22:48:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:48:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:48:17 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:48:18 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:48:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:48:29 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:48:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760805deb1a123f70f866680db67bfa3dcb8847b6ba0a19aa81db56e389e2fc0`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 4.4 MB (4364947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07edca5c09c7a639b08f5873160d9f51a67dca693c553c77bd4da3a487cf98b1`  
		Last Modified: Sat, 01 Feb 2020 22:57:59 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531ca140aa96954bbf71328b29b544b3a2e6d65750bde462ebaf5ceb9211a2f3`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 1.3 MB (1274917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5387f07d48aa567c90a5f600a88d52a3e23731fc526fe455615270e71eb87826`  
		Last Modified: Sat, 01 Feb 2020 22:57:57 GMT  
		Size: 6.2 MB (6185756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df00257572bca93ee8879d856b2ad35f675ee82aa6091ca73d467ca3743f67ed`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 293.5 KB (293536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d078612d1275942888b21d29cab572493f1e313c54b050434dcd70e2d76d544`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2e5ca1d60f37146aeff96ecb4c62cbe26cf5ebc72cb162751de46927921192`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0002035012ee6890ccde192d4b8382739b92a74d7c85020963046efc6c5bcd17`  
		Last Modified: Sat, 01 Feb 2020 22:59:06 GMT  
		Size: 52.8 MB (52772968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46e454b022b67067d2501e2bf6e71e8026a96ce04ec0188a00c5b5be5855fa4`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 7.8 KB (7833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50e5ae5b23eb887386d3d0d1902a9c59f0f7188a1a9f60a8d6856c4c0fc16d8`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f879a88c785812c8459cb56b4e86361265724a90985bf2f3550602a04c300bb6`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c088fbc21c50d68a5735d71d1d46b17da2caf2178d8b9670fdebd525d5d17117`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 3.8 KB (3845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9451f99ea65c745ef67c24042b50919eae46e00b0841446566dee9fed0d365f8`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; s390x

```console
$ docker pull postgres@sha256:4c6b34f3acfccb569d33132e5ad4479fdc089a26d798c424ede97d837d77932a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.3 MB (88297071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad50f8eb12b75d3c44dcc6af7f32ad5f92dc07b05847933aa1e9ee5c9774bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:55 GMT
ADD file:cf4bb119f25d8a9b9a2cd43101d5e87e0dbaa42d3f6688b39e66eea637225cc2 in / 
# Sat, 01 Feb 2020 16:43:57 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:40:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:40:14 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:40:23 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:40:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:40:28 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:40:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:40:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:55:32 GMT
ENV PG_MAJOR=9.6
# Sat, 01 Feb 2020 21:55:33 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sat, 01 Feb 2020 22:02:08 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:02:11 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:02:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:02:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sat, 01 Feb 2020 22:02:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:02:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:02:13 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:02:13 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:02:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:02:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:02:14 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:02:15 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:24a7c24214752593c0f651c56554e1bc6056ce340eb46cb71ed7ff0c430845a8`  
		Last Modified: Sat, 01 Feb 2020 16:47:44 GMT  
		Size: 22.4 MB (22380184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba584ff8c21579486e3687e8a4f6d0ecc911f32353708e9693752a64526d34f8`  
		Last Modified: Sat, 01 Feb 2020 22:15:15 GMT  
		Size: 4.5 MB (4534611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437afaa09e73336a77de2eaf796fdf66bd35380394ac42d0840b500f8a4972df`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1625730f985442686e8bba703b5a2f74d8ebb56b6c3f09d255ee5520ae0b83a`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.3 MB (1340980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505f199fff79fe4eb15264a3e92774fffb954fa9ca0b399800fafb2991aba6ea`  
		Last Modified: Sat, 01 Feb 2020 22:15:13 GMT  
		Size: 6.2 MB (6209613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea830cdc46d22c2ae31a6b440834f2563d2e28b2548c24b1daac41d82482f5f4`  
		Last Modified: Sat, 01 Feb 2020 22:15:11 GMT  
		Size: 294.6 KB (294550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c761a50d986b42286d1616f6bb992a8469b97207f4b48e434a5b6a81e2fe6`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc1bb55d92f21306a95cb3259eec2a3f3659245aeebb728d6698b7be3381b8`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54701b00a2872abeaf7e53c507b139529edc55392fb9fd1e730faf75bb833e2f`  
		Last Modified: Sat, 01 Feb 2020 22:16:13 GMT  
		Size: 53.5 MB (53518265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4e19a6f21d1cbb059a3eb3396945ebb64445c7acec95f0a20fd2a279068114`  
		Last Modified: Sat, 01 Feb 2020 22:16:03 GMT  
		Size: 7.8 KB (7819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e850dc1856bbd7bf63f47d449e8419ddc3e1da8fd9d3ccdea56cf30613fd42`  
		Last Modified: Sat, 01 Feb 2020 22:16:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375da53893bc523d68007c4526135647aefbac3618bc070b81abeed42a188921`  
		Last Modified: Sat, 01 Feb 2020 22:16:34 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f59d9757749cc559a6c6075fe6d6e5ed5a0c4f85094ef695cc153b7bddd2f8`  
		Last Modified: Sat, 01 Feb 2020 22:16:34 GMT  
		Size: 3.8 KB (3847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c09fda018d62ac9c322bee2a8ed2ee56e56f5b5780d6e43e669678efc414be`  
		Last Modified: Sat, 01 Feb 2020 22:16:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.4`

```console
$ docker pull postgres@sha256:d6bc1739199cc52f038f54e1ab671f5229d114fb667e9ad08add6cd66e8a9b28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:9.4` - linux; amd64

```console
$ docker pull postgres@sha256:dcb750a78d790b73bfd3e4d657b59375598072dd2b0151ef3226399abfa86972
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86641337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6046fc0afb442ecb26ddaff89ffd47e8c2e443128505adde2de12366bdc1477d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 06:07:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 06:07:31 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 06:07:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 06:07:59 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 06:08:00 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 06:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:08:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 06:08:12 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 06:10:59 GMT
ENV PG_MAJOR=9.4
# Sun, 02 Feb 2020 06:11:00 GMT
ENV PG_VERSION=9.4.25-1.pgdg90+1
# Sun, 02 Feb 2020 06:11:35 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 06:11:36 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 06:11:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 06:11:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.4/bin
# Sun, 02 Feb 2020 06:11:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 06:11:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 06:11:40 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 06:11:40 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:11:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 06:11:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:11:42 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 06:11:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0fe6664f6bb5f06d5d0a9a68c99a68be052403c684a8ffd98e70f6256d8ca`  
		Last Modified: Sun, 02 Feb 2020 06:12:59 GMT  
		Size: 4.5 MB (4501301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7ba8f77640450af762ebf643f368663949425d1bd516521dd9c0022a65461`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 1.8 KB (1779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1155d037e2c8553fc58b2671c2e61ca9ee29c7f712dbfc66dc20e8ab549c6b`  
		Last Modified: Sun, 02 Feb 2020 06:12:58 GMT  
		Size: 1.4 MB (1351457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febcfb7f8870017ab69faa0a454aa6a1e3cfde53c46074d1aa3e6edaea01adcc`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 6.2 MB (6182941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c78c79412b5cb255309e404e829646cc509a10cf8f55b2a5043da04d706604c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 295.6 KB (295582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a35744405c5f473d3002c5451970e6ff78bcc5eb330eea1c5595cca6b32679e`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27717922e0679badf783f2aa3179d254bb023533caf48d859c3d29723401701c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8ebde0a697885089928d903b72add163a456476b416d230f0b151f00246111`  
		Last Modified: Sun, 02 Feb 2020 06:14:43 GMT  
		Size: 51.8 MB (51767051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d85e3365411df2b18b3cc27330aec3df992d378322742c3785fe0893bd14cd`  
		Last Modified: Sun, 02 Feb 2020 06:14:29 GMT  
		Size: 7.3 KB (7341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c802081bbe1e0f07107f6af26b8d172748bc7462085868e9aabe31b1a1ffc373`  
		Last Modified: Sun, 02 Feb 2020 06:14:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35abd4ea98b43c6b1eb2bf920c0ce8c42b7c8fffc1eb75afac84f6cd69d38b4`  
		Last Modified: Sun, 02 Feb 2020 06:14:28 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50335e43732852ea51ab9424e423a5b04c89498d7d717a85c16ef38a86529b49`  
		Last Modified: Sun, 02 Feb 2020 06:14:28 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c34d9ddebbe6c19c0b518a904b5f5d7ff50f6c57694ad2fa4ccd03440f26ea`  
		Last Modified: Sun, 02 Feb 2020 06:14:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4` - linux; arm variant v5

```console
$ docker pull postgres@sha256:2d0775e52f7fbaf671ce8be296f4844c96764382cecdf39ba6979756f7869024
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83153475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec96250ac4e1b94a2a20f23a66f38591d02c18f327cc3c0b88a2c636198e1c4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:53:57 GMT
ADD file:f0d179649cbf50028b5ecd832961cc332fb524c2f12fda6c8060c3c258208be6 in / 
# Sat, 01 Feb 2020 16:53:59 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:04:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 19:04:31 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 19:05:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 19:05:16 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 19:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 19:05:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 20:30:38 GMT
ENV PG_MAJOR=9.4
# Sat, 01 Feb 2020 20:30:40 GMT
ENV PG_VERSION=9.4.25-1.pgdg90+1
# Sat, 01 Feb 2020 20:49:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 20:49:47 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 20:49:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 20:49:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.4/bin
# Sat, 01 Feb 2020 20:49:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 20:49:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 20:49:52 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 20:49:53 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 20:49:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 20:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 20:49:56 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 20:49:57 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:03886a8604d1b5423798ee97917dcb9de4cfdfbb7c435a7988d5c5e69a78e3b7`  
		Last Modified: Sat, 01 Feb 2020 17:01:03 GMT  
		Size: 21.2 MB (21202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aaa01ea1502b56b5ebd804228ff2ea5ad2adf78d4797d7a6aa75903a7dc7a30`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 4.2 MB (4236888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feeb9ed754ebd60d2d8cdffa636ff7e5b6ea1b1f68fd7c7aac5f1dced2f8cf9`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142683156b4ad1e2209ecaac30f55cd1a7237fe046f545e7a64613b34c221671`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.3 MB (1311293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950d1d965477d4d1230281bd3043f7347d94e263cada82cd86f3f055cc269e93`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 6.2 MB (6185421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1690d5dc7daff0def912cfa3c22eff87c80edb8f734454280c116e5fd52ebb92`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 293.5 KB (293479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0191375b3084722e33f875137d737673fc3ec09776716614c4fcd6764e7884e`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9bf11db5cc7dd3ff01824ff16d5642657294a22e3ec2086a5b3575ef803947`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 4.8 KB (4791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a915e3adad7cfd9dab621e41e8d8b29be8cd4daf83ab1faf59ca8ec094f30f`  
		Last Modified: Sat, 01 Feb 2020 20:53:13 GMT  
		Size: 49.9 MB (49905172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dcde38ee2da877e4997a76ef08536f74bf2b955f8430cd837172951d14ed0b`  
		Last Modified: Sat, 01 Feb 2020 20:52:51 GMT  
		Size: 7.3 KB (7346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ffeae6284d6426d44b26bac6cbef29dddc7e605638e96372028e2981dfc27c`  
		Last Modified: Sat, 01 Feb 2020 20:52:51 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1938dd66c54cac88ce59fa616c8bf6e52cf52908f7a769300f545445bd120664`  
		Last Modified: Sat, 01 Feb 2020 20:52:51 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82917d4093e3ffdbc22ed22be476a7fe1ccae8f33718386d91f802e11c800e75`  
		Last Modified: Sat, 01 Feb 2020 20:52:51 GMT  
		Size: 3.8 KB (3843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca3d19e12718190af7e8be7dd9b16d528445088da79945b5a7264ba9b8b5a7d`  
		Last Modified: Sat, 01 Feb 2020 20:52:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4` - linux; arm variant v7

```console
$ docker pull postgres@sha256:cc22bd8e4921ff4d7b739f21c5f6bdb4e2fd63de028be29197e34aea683fbcf0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79342798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d75107d9172ccdf46b9bc351b6a8e050cefc4928622665550fbcdfdfd7e1e34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 08:58:06 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 08:58:07 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 08:58:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 08:58:44 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 08:58:45 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 08:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:58:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 08:59:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 10:18:35 GMT
ENV PG_MAJOR=9.4
# Sun, 02 Feb 2020 10:18:37 GMT
ENV PG_VERSION=9.4.25-1.pgdg90+1
# Sun, 02 Feb 2020 10:35:05 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 10:35:10 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 10:35:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 10:35:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.4/bin
# Sun, 02 Feb 2020 10:35:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 10:35:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 10:35:16 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 10:35:17 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 10:35:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 10:35:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 10:35:20 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 10:35:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e359f7642afed089b2d05ece4e0736e03ceb13a937f7478eb868702665f809`  
		Last Modified: Sun, 02 Feb 2020 10:36:41 GMT  
		Size: 3.9 MB (3872826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b5742cb7fbb2cdb38f99c354efd420d24d27dee9b21b232dc92100066c10b`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6852094413bd98c461152c87837e91176b94a6cadae25e1a31b7f07330ecc4`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.3 MB (1303620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589bd77312350a872d2ebc5a6638ec844bf3aece0160a35b34a5d5cf66ae0d22`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 6.2 MB (6185708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943e832035ee98c3689f148b48e73550099b8f81fe37da09aa6e1ae2ea1756ac`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 291.9 KB (291867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba8ac21d907e788e2f05af094077cd10bcd20b8bb6eb5021b9f01ae1cfb1d97`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f8d5c6112a73a87453a9f3b2c2c298c0d2c275026fb63fb5ecdd81e6205461`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 4.8 KB (4792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9938aaa26bc8ef28d58257fc4331fea82731199aa4457fe52a1ff02cf0711d80`  
		Last Modified: Sun, 02 Feb 2020 10:38:44 GMT  
		Size: 48.4 MB (48358762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5c836e706d71bbbe737c4ec1193ff1e3a116c5cfafeb66869e695c2fc82ce4`  
		Last Modified: Sun, 02 Feb 2020 10:38:25 GMT  
		Size: 7.3 KB (7350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d221bbe97b92ca4d69bed422d7845c8faeb4224ca4e21555d2b66816584527f`  
		Last Modified: Sun, 02 Feb 2020 10:38:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0ffa58604715666a3abf0ab6af1cd2b609b55687abf1458d4893599b5adfd9`  
		Last Modified: Sun, 02 Feb 2020 10:38:25 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05751ef7794dd92973014d3b1188e5fa9dbcfd53a5312baa9a9bc1faa4f7e630`  
		Last Modified: Sun, 02 Feb 2020 10:38:25 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48ec793515c77750dfc741f5d1716b12a9fb7b975f9ab1f71baec48b8f5eb48`  
		Last Modified: Sun, 02 Feb 2020 10:38:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:52732d5a85331557682d5f8ae8c18ae55d562e9db724e8931e21d8598408c34a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82188109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efdc90bd451bdc0094b7a933038608e76d508a571892920df446d6b88d7996ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:24:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 02:24:24 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 02:24:27 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 02:24:52 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 02:25:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 02:25:09 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 02:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:25:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 02:25:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 03:48:18 GMT
ENV PG_MAJOR=9.4
# Sun, 02 Feb 2020 03:48:19 GMT
ENV PG_VERSION=9.4.25-1.pgdg90+1
# Sun, 02 Feb 2020 04:05:38 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 04:05:47 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 04:05:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 04:05:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.4/bin
# Sun, 02 Feb 2020 04:05:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 04:05:55 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 04:05:56 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 04:05:57 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 04:05:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 04:06:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 04:06:01 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 04:06:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a29899232ff5984832260695109c206ed14783ab8a33dd8f593f40672e2cf51`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 4.1 MB (4077687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72390476b7ab26db4e6e224ad16f9c0a3d66dce6b4d9996f6edece0992dec78e`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4470eb370695bb8691186ee389e7be5deaeb4f0d84a84ca948ae39ea977a1`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.3 MB (1286440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b51db6dc34b50eff6b5d8120f3efff4e5269216d5ea5d004ce80782e7508411`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 6.2 MB (6185392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918217c35d15c52bb58861e8c65a6b6934bc554387043c67b630758273c41028`  
		Last Modified: Sun, 02 Feb 2020 04:07:20 GMT  
		Size: 292.1 KB (292139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea01905f4f686b651e994714cb840779b241fcf43c04c6cc2a0ae229543862dc`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ff0687a25d7e24b75be4e353f57d8821a81a4b8c51aff2a01f927bb70d1a76`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 4.8 KB (4794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e901cfab699b34cc99b1a8533ea0d4ba343bf4c73a8cb70822732c4143db5f33`  
		Last Modified: Sun, 02 Feb 2020 04:09:22 GMT  
		Size: 49.9 MB (49942199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e753a049942015adbf57a2af4c3ed1dcd878ccf3cce05308396c3cdec5ace`  
		Last Modified: Sun, 02 Feb 2020 04:09:03 GMT  
		Size: 7.3 KB (7349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99600065acb165a8e84f0165421a07f91079dd67e5e07dfd28ddc82b01ab9921`  
		Last Modified: Sun, 02 Feb 2020 04:09:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f77742aac0a5273fac1d796400a215fbf2cd39db3f9311712773c373c18fd3`  
		Last Modified: Sun, 02 Feb 2020 04:09:03 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68097617ce9c3c8d5143a0235f110cf1c8b9ef42c6e3f085eb3244c029c0ed7c`  
		Last Modified: Sun, 02 Feb 2020 04:09:03 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f63fdc9f201ae881c1ec7713d47afdd6f8cd622e1fcd020eccdc79255d2d9b`  
		Last Modified: Sun, 02 Feb 2020 04:09:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4` - linux; 386

```console
$ docker pull postgres@sha256:6fc51ef956d19771b7036d20b937bc372cf422a9820e24d689d3f2d38aceaf11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87970701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0730b5bb81e6441dae8806ffc104884a61c9ca6c45ba340cefceea6892eb7a20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:21:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:21:11 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:21:27 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:21:39 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:21:39 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:21:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:21:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:21:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:25:54 GMT
ENV PG_MAJOR=9.4
# Sat, 01 Feb 2020 21:25:54 GMT
ENV PG_VERSION=9.4.25-1.pgdg90+1
# Sat, 01 Feb 2020 21:26:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:26:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:26:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:26:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.4/bin
# Sat, 01 Feb 2020 21:26:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:26:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:26:25 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:26:26 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:26:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:26:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:26:27 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:26:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400715a0cf80a4163f9bdfb01029e10c149b8ff3ce6ef1248f400451f617b081`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 4.8 MB (4807817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57223b59a38681596adf27043fcaa0c4896293e4b8d488d81957c76d11ee0d7`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb13941b5f12a8251a7c85981cb0d44069be9f4d1644bc34a11ae761968abdd8`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.3 MB (1318016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ada6bc6e6f24824fc92e6f96abb0ec680d29443a640d4b03d2ac54a6cb74ba`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 6.2 MB (6182955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65761eaa1a3239dc440a674c9a27612170189ab04f41d5360678cc34ddfab827`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 296.8 KB (296752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81305139d5a6d74e0ed5bf9ba0163f5c6baf0c66890f74d05e94b5313a57d86e`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ff425a04fcdc853777162926c616c569257ea00e96154204e9e3f91e2f7527`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb1927e98e9dade84b920f9cf2e0d802bd4d103ec2705a305cbec5a50d9c255`  
		Last Modified: Sat, 01 Feb 2020 21:30:01 GMT  
		Size: 52.2 MB (52194719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662045729befcdad01182a1e0d3b45dc3fbc6cabb5ad755a9a4dcc260eb8b800`  
		Last Modified: Sat, 01 Feb 2020 21:29:44 GMT  
		Size: 7.3 KB (7347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0620aaa88631e84b44127fab9393095dd93f9dc704b2297585955fb118cb1c51`  
		Last Modified: Sat, 01 Feb 2020 21:29:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97effd69451c85fb6b5336803011fd75f7f4fdac6d58c7e7dbae84060701c8b`  
		Last Modified: Sat, 01 Feb 2020 21:29:44 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac4fc4d775f4b4f9827a87d132e91f8a6624fc828462faee158b63899feef5f`  
		Last Modified: Sat, 01 Feb 2020 21:29:43 GMT  
		Size: 3.8 KB (3845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb1e700c81c86a8d8e0e3f35ba20917d67b6de91b1eb01a8f2791a6d17356b7`  
		Last Modified: Sat, 01 Feb 2020 21:29:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4` - linux; ppc64le

```console
$ docker pull postgres@sha256:572f56d39fa25de590e8d9dcf104e9df7079c55af1c6132c69dbf7505d8b0cba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.4 MB (86375376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f5746cd80e02e2293b7f21ff26901f576bdca9517edb3d99dd74b23c4aa387c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:34:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 22:34:47 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 22:34:48 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 22:35:35 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 22:35:55 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 22:35:58 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 22:36:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:36:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 22:36:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:52:50 GMT
ENV PG_MAJOR=9.4
# Sat, 01 Feb 2020 22:52:55 GMT
ENV PG_VERSION=9.4.25-1.pgdg90+1
# Sat, 01 Feb 2020 22:55:34 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:55:46 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:55:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:56:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.4/bin
# Sat, 01 Feb 2020 22:56:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:56:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:56:19 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:56:22 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:56:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:56:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:56:35 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:56:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760805deb1a123f70f866680db67bfa3dcb8847b6ba0a19aa81db56e389e2fc0`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 4.4 MB (4364947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07edca5c09c7a639b08f5873160d9f51a67dca693c553c77bd4da3a487cf98b1`  
		Last Modified: Sat, 01 Feb 2020 22:57:59 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531ca140aa96954bbf71328b29b544b3a2e6d65750bde462ebaf5ceb9211a2f3`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 1.3 MB (1274917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5387f07d48aa567c90a5f600a88d52a3e23731fc526fe455615270e71eb87826`  
		Last Modified: Sat, 01 Feb 2020 22:57:57 GMT  
		Size: 6.2 MB (6185756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df00257572bca93ee8879d856b2ad35f675ee82aa6091ca73d467ca3743f67ed`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 293.5 KB (293536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d078612d1275942888b21d29cab572493f1e313c54b050434dcd70e2d76d544`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2e5ca1d60f37146aeff96ecb4c62cbe26cf5ebc72cb162751de46927921192`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0eb1075e8cfefe7036d78ecb142589ad716d2632ba5d41db93a5a387af9e4c1`  
		Last Modified: Sat, 01 Feb 2020 23:00:03 GMT  
		Size: 51.4 MB (51437068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b703b378e544e92820d463a49d1b83ded4fab8e4dba35028fcefe8353e029b99`  
		Last Modified: Sat, 01 Feb 2020 22:59:47 GMT  
		Size: 7.3 KB (7344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b357fa44c02aeb100a9561991410ac505a856424ea73006d72242b540b6b9b67`  
		Last Modified: Sat, 01 Feb 2020 22:59:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bafd92bc7d482ac2218f18866067ee4896dfc0ecfc303fa1bfe2f7de786c5fd`  
		Last Modified: Sat, 01 Feb 2020 22:59:48 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cf2c0a6cce3e26e0182b53dcf826e9fb36ba725796203c14fe6a0b5204a7bf`  
		Last Modified: Sat, 01 Feb 2020 22:59:47 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2164bd924b84439a9e7944a3d91eeea44a2a20cbac096ab518616c9fd55a71`  
		Last Modified: Sat, 01 Feb 2020 22:59:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4` - linux; s390x

```console
$ docker pull postgres@sha256:6a701a5cb1386e05572fd8fdb7be9ef2357679c23f7c415577b170bf993f2761
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.9 MB (86938411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98a1bac305d1a0350fc3bd70c9ded99bc22de8605894180e32a369f92f531d9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:55 GMT
ADD file:cf4bb119f25d8a9b9a2cd43101d5e87e0dbaa42d3f6688b39e66eea637225cc2 in / 
# Sat, 01 Feb 2020 16:43:57 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:40:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:40:14 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:40:23 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:40:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:40:28 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:40:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:40:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:08:40 GMT
ENV PG_MAJOR=9.4
# Sat, 01 Feb 2020 22:08:41 GMT
ENV PG_VERSION=9.4.25-1.pgdg90+1
# Sat, 01 Feb 2020 22:14:13 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:14:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:14:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:14:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.4/bin
# Sat, 01 Feb 2020 22:14:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:14:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:14:18 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:14:18 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:14:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:14:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:14:19 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:14:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:24a7c24214752593c0f651c56554e1bc6056ce340eb46cb71ed7ff0c430845a8`  
		Last Modified: Sat, 01 Feb 2020 16:47:44 GMT  
		Size: 22.4 MB (22380184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba584ff8c21579486e3687e8a4f6d0ecc911f32353708e9693752a64526d34f8`  
		Last Modified: Sat, 01 Feb 2020 22:15:15 GMT  
		Size: 4.5 MB (4534611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437afaa09e73336a77de2eaf796fdf66bd35380394ac42d0840b500f8a4972df`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1625730f985442686e8bba703b5a2f74d8ebb56b6c3f09d255ee5520ae0b83a`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.3 MB (1340980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505f199fff79fe4eb15264a3e92774fffb954fa9ca0b399800fafb2991aba6ea`  
		Last Modified: Sat, 01 Feb 2020 22:15:13 GMT  
		Size: 6.2 MB (6209613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea830cdc46d22c2ae31a6b440834f2563d2e28b2548c24b1daac41d82482f5f4`  
		Last Modified: Sat, 01 Feb 2020 22:15:11 GMT  
		Size: 294.6 KB (294550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c761a50d986b42286d1616f6bb992a8469b97207f4b48e434a5b6a81e2fe6`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc1bb55d92f21306a95cb3259eec2a3f3659245aeebb728d6698b7be3381b8`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50c45df657b7213796f2d61326f80e24c07f9d050873c7bc12d3c825bb30a77`  
		Last Modified: Sat, 01 Feb 2020 22:17:10 GMT  
		Size: 52.2 MB (52160082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c48281503a63f563536ebca9930221496ecc3f22524dedaacea26b19417797`  
		Last Modified: Sat, 01 Feb 2020 22:17:01 GMT  
		Size: 7.3 KB (7342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ea8372a3a7c235b61d0c4645b50624d9070812c566559e80b7e0ea3f5726a3`  
		Last Modified: Sat, 01 Feb 2020 22:17:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f32c11ef44077209d07ec6fe3d5e5a4589e0d5c0ffa1ee650badabe6f51ef6a`  
		Last Modified: Sat, 01 Feb 2020 22:17:17 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25e9adde6d6bb5ae2ec76f0ad95490b424351758a37ec62c6ae44491d6659b7`  
		Last Modified: Sat, 01 Feb 2020 22:17:16 GMT  
		Size: 3.8 KB (3845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd30936025cfa89e527f4d79ad0b3ef6e547ba9b6121ff454b56f8930116ddb2`  
		Last Modified: Sat, 01 Feb 2020 22:17:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.4.26`

**does not exist** (yet?)

## `postgres:9.4.26-alpine`

**does not exist** (yet?)

## `postgres:9.4-alpine`

```console
$ docker pull postgres@sha256:77b9ed89c77b1fd279cab01b6da1b3fa25fa6b56bde61454d4e9899f92e2d498
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:9.4-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:c853dfc0f19d194a63361c1e1f461090018556a39e9e64a5ef53dc72525db8d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14221221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4f710a5561e8dc79b444deecc1f869061ef8a2577d02644b2b7a7b124ad2f98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:19:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:19:59 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:40:01 GMT
ENV PG_MAJOR=9.4
# Thu, 30 Jan 2020 03:40:02 GMT
ENV PG_VERSION=9.4.25
# Thu, 30 Jan 2020 03:40:02 GMT
ENV PG_SHA256=cb98afaef4748de76c13202c14198e3e4717adde49fd9c90fdc81da877520928
# Thu, 30 Jan 2020 03:42:25 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:42:26 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:42:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:42:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:42:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:42:28 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:42:28 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:42:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:42:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:42:29 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:42:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1030c456d04636112fa347ddc5296036cddf70c8085be2e3f3fb481898f18fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d0211bbd9a4fd28f739a797600d78394b15d947a30f55f70cfd5daf0f9e443`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7770fe83b180fe39acfa3169a670529f98a2855073fef45a2998c830e6ee82a7`  
		Last Modified: Thu, 30 Jan 2020 03:43:49 GMT  
		Size: 11.4 MB (11405964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fef6b8e64801071d0e5e22a4246b4fa60cab67b89bf7b5f5a773e9a6115a21`  
		Last Modified: Thu, 30 Jan 2020 03:43:46 GMT  
		Size: 6.7 KB (6686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416de68c3c636033989e6795f0bbf174011140542aca7bdfd6681eef4cd68a04`  
		Last Modified: Thu, 30 Jan 2020 03:43:46 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ed5c16a3b00d193424f899750c035e948796399333bd097f657f23bc732485`  
		Last Modified: Thu, 30 Jan 2020 03:43:46 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b29341985be92833b544a6b14bd23b9a733d9ec4a1ab31d2f59a9ae33d9b956`  
		Last Modified: Thu, 30 Jan 2020 03:43:46 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2375facf43606ddd4b6c2526021715a1a6b00f7bc91eadef830f12bb17d759d`  
		Last Modified: Thu, 30 Jan 2020 03:43:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:f6572bf8324365787eee25dd48e3ef3272bde1243b5e7b0fa32a794bc9d9aa69
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13643959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb607b07db2eff894b2162260a4075d2c103d3a9a6f027babfe44918299b433`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:49:35 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:49:36 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:49:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:08:48 GMT
ENV PG_MAJOR=9.4
# Thu, 30 Jan 2020 03:08:48 GMT
ENV PG_VERSION=9.4.25
# Thu, 30 Jan 2020 03:08:49 GMT
ENV PG_SHA256=cb98afaef4748de76c13202c14198e3e4717adde49fd9c90fdc81da877520928
# Thu, 30 Jan 2020 03:11:13 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:11:16 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:11:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:11:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:11:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:11:21 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:11:21 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:11:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:11:25 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:11:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab27e2422be886bc0a338b0e0c20b8e2beea15b880defbac81f75c04495d0c2`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae2520a8d4cdac962b6d4a62335dce896f8ccb0b6d2693b0e72591fda026d14`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42da1862727c670740e873de4efd7d3c39c7f08e5d2722dc7d3e987028d9dd9`  
		Last Modified: Thu, 30 Jan 2020 03:13:37 GMT  
		Size: 11.0 MB (11013970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1fe9ee96a022af428e3373d5fed48ab9702a3f45e63822e51a55049345afea`  
		Last Modified: Thu, 30 Jan 2020 03:13:31 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f228131e1073776ff96d2d61550e3c9dbd47e70206f397e6e550ec8ab942c8`  
		Last Modified: Thu, 30 Jan 2020 03:13:31 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b5d722bd44217cc6cec94dba7e84c601e6c237a0e8fb84a91be66980a4874e`  
		Last Modified: Thu, 30 Jan 2020 03:13:31 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51954b7fdf6cd593d6164aa97b887e42cfebe1418d153faf474ad04b5ba99269`  
		Last Modified: Thu, 30 Jan 2020 03:13:31 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3d46ef0916ff942e013b6bf4f7254a6d3554b0c5e912484cfa85702d284649`  
		Last Modified: Thu, 30 Jan 2020 03:13:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:4c96dc05ac7eb248ab5511c2756863a80725c662c929cc34a7df91b40fff27b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.8 MB (12842416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16cc6ae6519ceddd98b4c1ea28414b3f34a748042a9d76293543c25977f72242`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:00:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:00:13 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:00:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:15:25 GMT
ENV PG_MAJOR=9.4
# Thu, 30 Jan 2020 03:15:26 GMT
ENV PG_VERSION=9.4.25
# Thu, 30 Jan 2020 03:15:26 GMT
ENV PG_SHA256=cb98afaef4748de76c13202c14198e3e4717adde49fd9c90fdc81da877520928
# Thu, 30 Jan 2020 03:17:18 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:17:21 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:17:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:17:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:17:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:17:25 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:17:26 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:17:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:17:28 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:17:29 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572777a7d0992ea05b14f2ba3230ce906c753dd21eb73ac2b6018551250312db`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8810228251d658112d3dbf2b9b1719f402a0c3477bf2eceaa5a20341bba3f5`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1742e5f6770829062699ab5ac305020bc20231bbeec032672cd7f240937c646`  
		Last Modified: Thu, 30 Jan 2020 03:20:27 GMT  
		Size: 10.4 MB (10410433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac01c41c089812007fe99666f3d956a87e4d1038afefc714e3b44dc55c54679c`  
		Last Modified: Thu, 30 Jan 2020 03:20:22 GMT  
		Size: 6.7 KB (6692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ffa15a7be34d4154bd125229155edd382163fb2f5cb0f74a71f7ed65bbb7b8`  
		Last Modified: Thu, 30 Jan 2020 03:20:22 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182869f11b5849c70d17c3c83d10b29648df44997708a9fdfc2a7d8bbb84498e`  
		Last Modified: Thu, 30 Jan 2020 03:20:22 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8dafece34b3e9c59f001b6c729e873a41a36e4af98520d92962f350bde8b4e`  
		Last Modified: Thu, 30 Jan 2020 03:20:23 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddd8ac7f3f05d9b227d7eebf9961c26a14f29df644a0d5b412772eac7f341e2`  
		Last Modified: Thu, 30 Jan 2020 03:20:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:a1d9fa1bbaf18c09671d3ec5264d51384c48e7e9f159b6d6b6650efa4b74cf43
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13991988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58a4bace8338cc535c07bfca77d949aaaac09efe894256cab69badf5ac430d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:40:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:40:28 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:56:59 GMT
ENV PG_MAJOR=9.4
# Thu, 30 Jan 2020 02:56:59 GMT
ENV PG_VERSION=9.4.25
# Thu, 30 Jan 2020 02:57:00 GMT
ENV PG_SHA256=cb98afaef4748de76c13202c14198e3e4717adde49fd9c90fdc81da877520928
# Thu, 30 Jan 2020 02:59:08 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:59:13 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:59:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:59:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:59:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:59:19 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:59:20 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:59:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:59:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:59:24 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:59:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db837ff5778a13ace9e439e3bff33c317ecca84803a142a4ee4e05d2af54def`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92b445ab1ef4ba9a6120e5cc359b70cb88b74a46dee803f2709cb873a7be79`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5dac791196f31bf9dca078d9fe9d6145b2702de217d975ed8ed443b71d81f34`  
		Last Modified: Thu, 30 Jan 2020 03:01:36 GMT  
		Size: 11.3 MB (11256492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb63fd8781fe557a9fbc71cb68e66298503cda890dd0774471406bc1c18d7dd`  
		Last Modified: Thu, 30 Jan 2020 03:01:30 GMT  
		Size: 6.7 KB (6684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1039f6588d24d2b110aec06b4e066649105af68852049448ab7692a61c0113bb`  
		Last Modified: Thu, 30 Jan 2020 03:01:30 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e108b4d9ffb3c4f722365b3c44c83fa159feb14f9c8b9fab461c363b158aea7`  
		Last Modified: Thu, 30 Jan 2020 03:01:30 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4837754ead341cdf558e29f7cb87cfca334bebdf8c576602aa1656a11f1e381a`  
		Last Modified: Thu, 30 Jan 2020 03:01:30 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7145ac82ef390554476d6c7dc2406628592243f0fa4cbf18f7e95a28746b023`  
		Last Modified: Thu, 30 Jan 2020 03:01:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4-alpine` - linux; 386

```console
$ docker pull postgres@sha256:c49a3a0b1009267b5d4dac48435c78a1d2ed0145cd4c54949e75aa0d7c6b838d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14801432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55a2b99de6409a8e532e545b326bad5231237090e7de453e2956237d1629fb82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:38:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:38:44 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:38:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:03:34 GMT
ENV PG_MAJOR=9.4
# Thu, 30 Jan 2020 03:03:34 GMT
ENV PG_VERSION=9.4.25
# Thu, 30 Jan 2020 03:03:35 GMT
ENV PG_SHA256=cb98afaef4748de76c13202c14198e3e4717adde49fd9c90fdc81da877520928
# Thu, 30 Jan 2020 03:06:42 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:06:43 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:06:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:06:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:06:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:06:45 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:06:45 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:06:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:06:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:06:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:06:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb8463eb063fd24e3d29bd4ca5b9ba1590717acda7415cb45da3e7560f0dd`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023c33adbfeb9b779f40edac1617b4514e1fb0b976b5b201dd0f7dc688f5e60`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e1da43f070b238d41fc013e87bf7acd28cc092e2a428292ac22daddbade43b`  
		Last Modified: Thu, 30 Jan 2020 03:08:29 GMT  
		Size: 12.0 MB (11982573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dd8ca82824cb6a9f1a01f40fb1600ddcd5a7e54444211d2a41425af7a9fd54`  
		Last Modified: Thu, 30 Jan 2020 03:08:24 GMT  
		Size: 6.7 KB (6690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8433ada357ed50355484a4062a80432e5a5ac5f0ec14873d694b401f8a4285`  
		Last Modified: Thu, 30 Jan 2020 03:08:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbbbf227a336cdb8c837addba93f98cfb7761303c805d78f2ddd03c6402d1af`  
		Last Modified: Thu, 30 Jan 2020 03:08:24 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b19c62cb66b64d928f67c8d18f4c721fe1ee850704b672e92944f37e583e2a`  
		Last Modified: Thu, 30 Jan 2020 03:08:24 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa31ba6a6bda8d6ca2fc7a83db9d7ea0fe10da3c693607981e2d91bac32bedb`  
		Last Modified: Thu, 30 Jan 2020 03:08:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:4d2ead9f0b48373c367bda8aacdd4411b638bdfbc374331f5b23404832224a71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15101955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7123c349da8e5f501014aad976a367b6816ce6e786eb5b9a4f16cd4399ec011b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:20:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:20:03 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:48:08 GMT
ENV PG_MAJOR=9.4
# Thu, 30 Jan 2020 03:48:12 GMT
ENV PG_VERSION=9.4.25
# Thu, 30 Jan 2020 03:48:14 GMT
ENV PG_SHA256=cb98afaef4748de76c13202c14198e3e4717adde49fd9c90fdc81da877520928
# Thu, 30 Jan 2020 03:51:55 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:52:03 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:52:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:52:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:52:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:52:28 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:52:29 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:52:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:52:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:52:43 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:52:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8af198a4c612619984a3d16dc2a9fb3f15835dfbf5269a9eab9a345ed4f14`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852af7c4759ead6b82b170b6d34d124532026b41ec5d7dc4ec99bd6705f633a`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b142c8ba9a66dca0ff7a2b40f5c6e5910103ee0c9417d1ed81e8f15c4118c845`  
		Last Modified: Thu, 30 Jan 2020 03:55:17 GMT  
		Size: 12.3 MB (12267411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a987990ff5c02c513686976005ae9a1b384e0c7c44dbf2f1611e79e9f89340`  
		Last Modified: Thu, 30 Jan 2020 03:55:11 GMT  
		Size: 6.7 KB (6683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d9a71dba760fbd899582df76ba90fd8b89ade5331fc14a76398786e417c93f`  
		Last Modified: Thu, 30 Jan 2020 03:55:11 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41144fbc57425699949220ee80fb66a59a38d2086a4ac0f9282ea2ead174a73a`  
		Last Modified: Thu, 30 Jan 2020 03:55:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188b595dc39a4419889e40698124b4157b4703cf6f36161c3d9890bd551f69f`  
		Last Modified: Thu, 30 Jan 2020 03:55:11 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cbb456d78ec1eac8d08514515d4d689f1cd017493fedaa41b52b9b83887554`  
		Last Modified: Thu, 30 Jan 2020 03:55:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.4-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:ca716d5a17035fa985ba4133f3aa7512c090f7a53135ee46d4bc60c950638616
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13833353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a002039f7aad130ad50592a7b2a1c4299f205fa33ad07677ebbe9904e5ece786`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:48:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:48:56 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:48:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:04:57 GMT
ENV PG_MAJOR=9.4
# Thu, 30 Jan 2020 03:04:57 GMT
ENV PG_VERSION=9.4.25
# Thu, 30 Jan 2020 03:04:57 GMT
ENV PG_SHA256=cb98afaef4748de76c13202c14198e3e4717adde49fd9c90fdc81da877520928
# Thu, 30 Jan 2020 03:06:53 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:06:55 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:06:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:06:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:06:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:06:56 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:06:56 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:06:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:06:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:06:57 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:06:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d0ab56996305262d42136eee090848bbdf7cec28b8625e39078668b245db48`  
		Last Modified: Thu, 30 Jan 2020 03:07:31 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd3ab8f7e8df3f56e9628a504d2ea6db996a9910565bf84e3bc35bd847bcfb`  
		Last Modified: Thu, 30 Jan 2020 03:07:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b9c5bc985e421f7b4c4003970c758a7c7bc0e6adb6f7fc45ab0925d41a2823`  
		Last Modified: Thu, 30 Jan 2020 03:08:47 GMT  
		Size: 11.2 MB (11238900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b595ed00c9ccfcc2cc033e5093e63f1906a1fa43f57c8efef9c390d0439fd3`  
		Last Modified: Thu, 30 Jan 2020 03:08:40 GMT  
		Size: 6.7 KB (6684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b3a57480b3c3e03543f733958243da3060d8b4f938d70d608054a4118dde0c`  
		Last Modified: Thu, 30 Jan 2020 03:08:45 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30d7e39c9c63b85590353745dbf76518d3cc8c1538b21839348a108a64cc22f`  
		Last Modified: Thu, 30 Jan 2020 03:08:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da29bfa436189b9f50a8c06d67f65a8907647d88ad8cc04f68c88c991eb847a1`  
		Last Modified: Thu, 30 Jan 2020 03:08:40 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9358f273b4f8e5ba0d3ab1cc9a1e3dba2bc0384bb959223f7e68b3ba07686815`  
		Last Modified: Thu, 30 Jan 2020 03:08:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.5`

```console
$ docker pull postgres@sha256:54a9f2c39fa0c7903bfb4d32568820a45bceb60a491e6378d35cc74b65be7b1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:9.5` - linux; amd64

```console
$ docker pull postgres@sha256:2ec532fa949a13ebe5841c74976706b7c9eb3e2c31aaf7955d0fd74e3bb6a81a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86998558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08e9a3b7f7bff1786a9826c87ddcde70e056b6cd44e4ecd1f95e9d1f7703744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 06:07:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 06:07:31 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 06:07:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 06:07:59 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 06:08:00 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 06:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:08:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 06:08:12 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 06:10:22 GMT
ENV PG_MAJOR=9.5
# Sun, 02 Feb 2020 06:10:22 GMT
ENV PG_VERSION=9.5.20-1.pgdg90+1
# Sun, 02 Feb 2020 06:10:46 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 06:10:47 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 06:10:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 06:10:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Sun, 02 Feb 2020 06:10:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 06:10:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 06:10:49 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 06:10:49 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:10:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 06:10:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:10:50 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 06:10:50 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0fe6664f6bb5f06d5d0a9a68c99a68be052403c684a8ffd98e70f6256d8ca`  
		Last Modified: Sun, 02 Feb 2020 06:12:59 GMT  
		Size: 4.5 MB (4501301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7ba8f77640450af762ebf643f368663949425d1bd516521dd9c0022a65461`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 1.8 KB (1779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1155d037e2c8553fc58b2671c2e61ca9ee29c7f712dbfc66dc20e8ab549c6b`  
		Last Modified: Sun, 02 Feb 2020 06:12:58 GMT  
		Size: 1.4 MB (1351457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febcfb7f8870017ab69faa0a454aa6a1e3cfde53c46074d1aa3e6edaea01adcc`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 6.2 MB (6182941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c78c79412b5cb255309e404e829646cc509a10cf8f55b2a5043da04d706604c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 295.6 KB (295582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a35744405c5f473d3002c5451970e6ff78bcc5eb330eea1c5595cca6b32679e`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27717922e0679badf783f2aa3179d254bb023533caf48d859c3d29723401701c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebd6ec05a24f58f73781fb4c11586b08a6b8a04e7eb10d5b478cea718b985fe`  
		Last Modified: Sun, 02 Feb 2020 06:14:23 GMT  
		Size: 52.1 MB (52124079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a12e41a30c5c20db0578c766ff5c10fc204a3fb7374a1705f84a65be6d95b9d`  
		Last Modified: Sun, 02 Feb 2020 06:14:07 GMT  
		Size: 7.5 KB (7534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6fd4a8e561e2e025526645f47111be68f9344f548fca74bb8dc7216b52d9c4`  
		Last Modified: Sun, 02 Feb 2020 06:14:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c470cc1fc3329b2418a484dfee1df3431f733b59491a3f0354818f96c4277f7`  
		Last Modified: Sun, 02 Feb 2020 06:14:07 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8895387da1b59a901ca55bbc538c11d644d1f1d78c7ef62b601c2c76675b326`  
		Last Modified: Sun, 02 Feb 2020 06:14:07 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ac611f04694681ba5be331bade5965704b89541eceeae642b5eabd8dc89c26`  
		Last Modified: Sun, 02 Feb 2020 06:14:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; arm variant v5

```console
$ docker pull postgres@sha256:f4790488017d8d7ceb220e20de324172cc65bb857661a747867948d5365bf7a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83504070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:839e7921ba98dd917d7b4156060a63eae8acbac3fd2d765fc547d885ed057f0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:53:57 GMT
ADD file:f0d179649cbf50028b5ecd832961cc332fb524c2f12fda6c8060c3c258208be6 in / 
# Sat, 01 Feb 2020 16:53:59 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:04:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 19:04:31 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 19:05:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 19:05:16 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 19:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 19:05:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 20:09:51 GMT
ENV PG_MAJOR=9.5
# Sat, 01 Feb 2020 20:09:51 GMT
ENV PG_VERSION=9.5.20-1.pgdg90+1
# Sat, 01 Feb 2020 20:30:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 20:30:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 20:30:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 20:30:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Sat, 01 Feb 2020 20:30:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 20:30:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 20:30:20 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 20:30:20 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 20:30:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 20:30:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 20:30:23 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 20:30:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:03886a8604d1b5423798ee97917dcb9de4cfdfbb7c435a7988d5c5e69a78e3b7`  
		Last Modified: Sat, 01 Feb 2020 17:01:03 GMT  
		Size: 21.2 MB (21202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aaa01ea1502b56b5ebd804228ff2ea5ad2adf78d4797d7a6aa75903a7dc7a30`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 4.2 MB (4236888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feeb9ed754ebd60d2d8cdffa636ff7e5b6ea1b1f68fd7c7aac5f1dced2f8cf9`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142683156b4ad1e2209ecaac30f55cd1a7237fe046f545e7a64613b34c221671`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.3 MB (1311293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950d1d965477d4d1230281bd3043f7347d94e263cada82cd86f3f055cc269e93`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 6.2 MB (6185421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1690d5dc7daff0def912cfa3c22eff87c80edb8f734454280c116e5fd52ebb92`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 293.5 KB (293479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0191375b3084722e33f875137d737673fc3ec09776716614c4fcd6764e7884e`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9bf11db5cc7dd3ff01824ff16d5642657294a22e3ec2086a5b3575ef803947`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 4.8 KB (4791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba435b89f6202591f22bf5c75eba63d7255cfeefb75217428089ed51f5569057`  
		Last Modified: Sat, 01 Feb 2020 20:52:44 GMT  
		Size: 50.3 MB (50255572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb3f113c19c0b8aff63e96fd6704a848cc7297494c3464abf3f625e518ad7c2`  
		Last Modified: Sat, 01 Feb 2020 20:52:24 GMT  
		Size: 7.5 KB (7538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38babccaeb1b7a3308e4d4c1a063c145fea47ebf37f4c9ceb0fe73fa85791c4e`  
		Last Modified: Sat, 01 Feb 2020 20:52:24 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006a416bd3582b7475215c0f656edd722fccc15c113bc60f016a409816383793`  
		Last Modified: Sat, 01 Feb 2020 20:52:24 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fdf43d3b901505a3e93d78059df5441cd617e38c8fa87c608e51192e8a2718`  
		Last Modified: Sat, 01 Feb 2020 20:52:24 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cc1d3aa3ff1ad67b7937778e2e07c01ed50b468c610d35037141aacfba8489`  
		Last Modified: Sat, 01 Feb 2020 20:52:24 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; arm variant v7

```console
$ docker pull postgres@sha256:2b72664174c63a7d46e4aed0267219274f8be46d98617f60a3ccf6a93ee8eed7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.7 MB (79667151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2920c45349ee258e35ad3def065a5dae07d5479a056be25255dc467cf9a67d0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 08:58:06 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 08:58:07 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 08:58:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 08:58:44 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 08:58:45 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 08:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:58:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 08:59:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 09:59:44 GMT
ENV PG_MAJOR=9.5
# Sun, 02 Feb 2020 09:59:45 GMT
ENV PG_VERSION=9.5.20-1.pgdg90+1
# Sun, 02 Feb 2020 10:17:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 10:18:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 10:18:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 10:18:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Sun, 02 Feb 2020 10:18:04 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 10:18:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 10:18:06 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 10:18:07 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 10:18:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 10:18:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 10:18:12 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 10:18:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e359f7642afed089b2d05ece4e0736e03ceb13a937f7478eb868702665f809`  
		Last Modified: Sun, 02 Feb 2020 10:36:41 GMT  
		Size: 3.9 MB (3872826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b5742cb7fbb2cdb38f99c354efd420d24d27dee9b21b232dc92100066c10b`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6852094413bd98c461152c87837e91176b94a6cadae25e1a31b7f07330ecc4`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.3 MB (1303620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589bd77312350a872d2ebc5a6638ec844bf3aece0160a35b34a5d5cf66ae0d22`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 6.2 MB (6185708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943e832035ee98c3689f148b48e73550099b8f81fe37da09aa6e1ae2ea1756ac`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 291.9 KB (291867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba8ac21d907e788e2f05af094077cd10bcd20b8bb6eb5021b9f01ae1cfb1d97`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f8d5c6112a73a87453a9f3b2c2c298c0d2c275026fb63fb5ecdd81e6205461`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 4.8 KB (4792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194559512e406371726e733356874a890e7b019af25347d0976f0e6f323835b3`  
		Last Modified: Sun, 02 Feb 2020 10:38:18 GMT  
		Size: 48.7 MB (48682931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbe08942cfba739e163472fbf9ebbd4bf40aa4bf4e379d2443670a4d5d339bf`  
		Last Modified: Sun, 02 Feb 2020 10:38:00 GMT  
		Size: 7.5 KB (7533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599a3c202f38998b6e2690eed261c551fc7aec505ec25d770360dbdeced6533c`  
		Last Modified: Sun, 02 Feb 2020 10:38:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c78dbf71858ded72b3fcf427084956b3d64ad85ed168dbaca02bb125c25a83`  
		Last Modified: Sun, 02 Feb 2020 10:38:00 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f4534c4c2cc2b684d44b32cab2407eb2d7c70428c265f91b7534c9631a2480`  
		Last Modified: Sun, 02 Feb 2020 10:38:00 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb376353c25f11e70d0d31288f7d091026a225784234620c6f69016cfcc54d6`  
		Last Modified: Sun, 02 Feb 2020 10:38:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:b02f01523d9f07f00fb7ba9d5d96b355ffdd4b6800589eac1764ca427240f87a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82513019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2596b2f938e36c7a093816cd23809682aaeb9d7b4aa1ee7d0d4f195ddd502bda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:24:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 02:24:24 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 02:24:27 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 02:24:52 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 02:25:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 02:25:09 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 02:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:25:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 02:25:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 03:28:56 GMT
ENV PG_MAJOR=9.5
# Sun, 02 Feb 2020 03:28:57 GMT
ENV PG_VERSION=9.5.20-1.pgdg90+1
# Sun, 02 Feb 2020 03:47:31 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 03:47:41 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 03:47:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 03:47:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Sun, 02 Feb 2020 03:47:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 03:47:55 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 03:47:56 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 03:47:57 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 03:48:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 03:48:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:48:02 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 03:48:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a29899232ff5984832260695109c206ed14783ab8a33dd8f593f40672e2cf51`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 4.1 MB (4077687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72390476b7ab26db4e6e224ad16f9c0a3d66dce6b4d9996f6edece0992dec78e`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4470eb370695bb8691186ee389e7be5deaeb4f0d84a84ca948ae39ea977a1`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.3 MB (1286440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b51db6dc34b50eff6b5d8120f3efff4e5269216d5ea5d004ce80782e7508411`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 6.2 MB (6185392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918217c35d15c52bb58861e8c65a6b6934bc554387043c67b630758273c41028`  
		Last Modified: Sun, 02 Feb 2020 04:07:20 GMT  
		Size: 292.1 KB (292139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea01905f4f686b651e994714cb840779b241fcf43c04c6cc2a0ae229543862dc`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ff0687a25d7e24b75be4e353f57d8821a81a4b8c51aff2a01f927bb70d1a76`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 4.8 KB (4794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af895d6e18520f0a50376eae2b2fb0207299528f99363f8b63163350bb387a32`  
		Last Modified: Sun, 02 Feb 2020 04:08:56 GMT  
		Size: 50.3 MB (50266926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bb1401c1756e515005c1e6308d13bf132ffe24d6073a77bc2836098c8ce42e`  
		Last Modified: Sun, 02 Feb 2020 04:08:37 GMT  
		Size: 7.5 KB (7533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36edae04891f1dce3da38969ea508b7094cdae81673dfac89a0016418861a319`  
		Last Modified: Sun, 02 Feb 2020 04:08:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1377b8a66c5b0f1ce7a5505f1182f2453b48012937f6ba63036086c154eecfd5`  
		Last Modified: Sun, 02 Feb 2020 04:08:37 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a204c48bb1860b0b4a172f7f729e72aa4f64525b1f4bcec2770a13db06b876a7`  
		Last Modified: Sun, 02 Feb 2020 04:08:38 GMT  
		Size: 3.8 KB (3847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3231425a79cbeca6325c5d4294a36e0937ae345e6bc511af45a26f4b2e929d`  
		Last Modified: Sun, 02 Feb 2020 04:08:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; 386

```console
$ docker pull postgres@sha256:64ab57df0aada8c7cf6843187f414b7c7e3a9982e452b70df71d0e7aa46cb03c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88354306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17175bb4056b9ef420ff39fa76a908d34ee9af7505776fd122ed08905269922b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:21:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:21:11 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:21:27 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:21:39 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:21:39 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:21:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:21:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:21:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:25:12 GMT
ENV PG_MAJOR=9.5
# Sat, 01 Feb 2020 21:25:12 GMT
ENV PG_VERSION=9.5.20-1.pgdg90+1
# Sat, 01 Feb 2020 21:25:38 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:25:39 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:25:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:25:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Sat, 01 Feb 2020 21:25:40 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:25:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:25:41 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:25:42 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:25:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:25:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:25:43 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:25:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400715a0cf80a4163f9bdfb01029e10c149b8ff3ce6ef1248f400451f617b081`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 4.8 MB (4807817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57223b59a38681596adf27043fcaa0c4896293e4b8d488d81957c76d11ee0d7`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb13941b5f12a8251a7c85981cb0d44069be9f4d1644bc34a11ae761968abdd8`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.3 MB (1318016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ada6bc6e6f24824fc92e6f96abb0ec680d29443a640d4b03d2ac54a6cb74ba`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 6.2 MB (6182955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65761eaa1a3239dc440a674c9a27612170189ab04f41d5360678cc34ddfab827`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 296.8 KB (296752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81305139d5a6d74e0ed5bf9ba0163f5c6baf0c66890f74d05e94b5313a57d86e`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ff425a04fcdc853777162926c616c569257ea00e96154204e9e3f91e2f7527`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae2e5c4586ecd6bedf7e28bdfbc8be48982ea53b4c878334a23349a0b8c1b9f`  
		Last Modified: Sat, 01 Feb 2020 21:29:39 GMT  
		Size: 52.6 MB (52578138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a96f7b513b83dca9a1646cb03c9cb42a04284dea544e730a4a1de9cced3869`  
		Last Modified: Sat, 01 Feb 2020 21:29:16 GMT  
		Size: 7.5 KB (7533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca24b7ab4056dbf7725f4b4d3a7a7097f7e6f0bccc160ab965b8ac8de194ae8`  
		Last Modified: Sat, 01 Feb 2020 21:29:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d148e09dd5392a4827c6364e4c64d5d82a9ddd3a15af61125413624e6390d4`  
		Last Modified: Sat, 01 Feb 2020 21:29:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f29cf3959d39a8de56a1accaada258134e142d7674ae2d7acad7f5fbb2d31b`  
		Last Modified: Sat, 01 Feb 2020 21:29:16 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42a76fcaea424b8a535a202238be743fcd82c54f80940e9b1eaf8e4af389b6c`  
		Last Modified: Sat, 01 Feb 2020 21:29:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; ppc64le

```console
$ docker pull postgres@sha256:20c7727155f0241013e45ec8228fc42976df0c8b5b026a041fc3c4b19e400075
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86724725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ca7a9ce053f8d76fe986720379279d43f0d01bc410dacca5619a52389754f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:34:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 22:34:47 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 22:34:48 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 22:35:35 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 22:35:55 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 22:35:58 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 22:36:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:36:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 22:36:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:48:47 GMT
ENV PG_MAJOR=9.5
# Sat, 01 Feb 2020 22:48:52 GMT
ENV PG_VERSION=9.5.20-1.pgdg90+1
# Sat, 01 Feb 2020 22:51:27 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:51:39 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:51:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:51:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Sat, 01 Feb 2020 22:51:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:52:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:52:05 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:52:07 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:52:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:52:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:52:22 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:52:25 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760805deb1a123f70f866680db67bfa3dcb8847b6ba0a19aa81db56e389e2fc0`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 4.4 MB (4364947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07edca5c09c7a639b08f5873160d9f51a67dca693c553c77bd4da3a487cf98b1`  
		Last Modified: Sat, 01 Feb 2020 22:57:59 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531ca140aa96954bbf71328b29b544b3a2e6d65750bde462ebaf5ceb9211a2f3`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 1.3 MB (1274917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5387f07d48aa567c90a5f600a88d52a3e23731fc526fe455615270e71eb87826`  
		Last Modified: Sat, 01 Feb 2020 22:57:57 GMT  
		Size: 6.2 MB (6185756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df00257572bca93ee8879d856b2ad35f675ee82aa6091ca73d467ca3743f67ed`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 293.5 KB (293536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d078612d1275942888b21d29cab572493f1e313c54b050434dcd70e2d76d544`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2e5ca1d60f37146aeff96ecb4c62cbe26cf5ebc72cb162751de46927921192`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3acf08cdee214d3dc61ec12de994cfe6c6dfc68ea85b18305dbbedb244a73a7`  
		Last Modified: Sat, 01 Feb 2020 22:59:36 GMT  
		Size: 51.8 MB (51786227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2b98f00be0eb9efa1df8bc066cbc40947af42a42f2ebcd4e1303a1999d05be`  
		Last Modified: Sat, 01 Feb 2020 22:59:20 GMT  
		Size: 7.5 KB (7533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c953bdfedf903561f9de24e8285a7f307167af168c1e3bc879bacee46707c29`  
		Last Modified: Sat, 01 Feb 2020 22:59:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b065e3c13eef405f7f7e0586b4a4178a0cdf02db04701aac8e0c05aedb2963`  
		Last Modified: Sat, 01 Feb 2020 22:59:21 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a1f25db1ec59f58c0bc812d24ddf1ff396b426e574ab4057e1836d3e5aa738`  
		Last Modified: Sat, 01 Feb 2020 22:59:20 GMT  
		Size: 3.8 KB (3843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b9228ae228ab15ee81291a742da1ce8764a445d8745e3110339b80166cf967`  
		Last Modified: Sat, 01 Feb 2020 22:59:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; s390x

```console
$ docker pull postgres@sha256:fd65ef93a75e9ffd9808407c4dc2980b0ba8e103199ba5616644c8f835b895c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.3 MB (87295308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acb78e44dc7e9447546e360321a084c4b8e19117cb6e52710bdde76ec21c1ed7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:55 GMT
ADD file:cf4bb119f25d8a9b9a2cd43101d5e87e0dbaa42d3f6688b39e66eea637225cc2 in / 
# Sat, 01 Feb 2020 16:43:57 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:40:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:40:14 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:40:23 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:40:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:40:28 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:40:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:40:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:02:28 GMT
ENV PG_MAJOR=9.5
# Sat, 01 Feb 2020 22:02:29 GMT
ENV PG_VERSION=9.5.20-1.pgdg90+1
# Sat, 01 Feb 2020 22:08:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:08:25 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:08:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:08:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Sat, 01 Feb 2020 22:08:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:08:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:08:27 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:08:27 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:08:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:08:28 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:08:28 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:24a7c24214752593c0f651c56554e1bc6056ce340eb46cb71ed7ff0c430845a8`  
		Last Modified: Sat, 01 Feb 2020 16:47:44 GMT  
		Size: 22.4 MB (22380184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba584ff8c21579486e3687e8a4f6d0ecc911f32353708e9693752a64526d34f8`  
		Last Modified: Sat, 01 Feb 2020 22:15:15 GMT  
		Size: 4.5 MB (4534611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437afaa09e73336a77de2eaf796fdf66bd35380394ac42d0840b500f8a4972df`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1625730f985442686e8bba703b5a2f74d8ebb56b6c3f09d255ee5520ae0b83a`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.3 MB (1340980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505f199fff79fe4eb15264a3e92774fffb954fa9ca0b399800fafb2991aba6ea`  
		Last Modified: Sat, 01 Feb 2020 22:15:13 GMT  
		Size: 6.2 MB (6209613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea830cdc46d22c2ae31a6b440834f2563d2e28b2548c24b1daac41d82482f5f4`  
		Last Modified: Sat, 01 Feb 2020 22:15:11 GMT  
		Size: 294.6 KB (294550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c761a50d986b42286d1616f6bb992a8469b97207f4b48e434a5b6a81e2fe6`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc1bb55d92f21306a95cb3259eec2a3f3659245aeebb728d6698b7be3381b8`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b704487470b3e7b601dea2e007b612a9cd07b188f6f2bc7f76b99538c737d7f`  
		Last Modified: Sat, 01 Feb 2020 22:16:54 GMT  
		Size: 52.5 MB (52516788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343e2015a116e88b1f308fa5bfe706aca05b3a0ac5cd7c9e37408a227dea284c`  
		Last Modified: Sat, 01 Feb 2020 22:16:40 GMT  
		Size: 7.5 KB (7533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f9d19890bba090da8c7721c4441ace0bd149ddcd16bf1e5bafbb8c62b60f7c`  
		Last Modified: Sat, 01 Feb 2020 22:16:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e18916cabbdc837d45acdd881960651df086608df4fed67c5daacd723e91de`  
		Last Modified: Sat, 01 Feb 2020 22:16:56 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49adbb741cd0f0ac4403326d5ba56e05940c3b67d1e92a0e10863d3d68f21453`  
		Last Modified: Sat, 01 Feb 2020 22:16:56 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70aa802414ede4397d6404abd0eff5992c3e8820493c46342b565237ad12769f`  
		Last Modified: Sat, 01 Feb 2020 22:16:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.5.21`

**does not exist** (yet?)

## `postgres:9.5.21-alpine`

**does not exist** (yet?)

## `postgres:9.5-alpine`

```console
$ docker pull postgres@sha256:bb33310d367c5a61bb54d72dc0ad2751e45ff734b122bf71e47b4044301c5903
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:9.5-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:e2c59935d8be96d7482cd7b6d190b47388dbc45d878ab65c628d418386254b21
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14367126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14bacaedfd9155599ad9944ca01298727e6e282371586cf56c56420bad2b4054`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:19:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:19:59 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:37:14 GMT
ENV PG_MAJOR=9.5
# Thu, 30 Jan 2020 03:37:14 GMT
ENV PG_VERSION=9.5.20
# Thu, 30 Jan 2020 03:37:14 GMT
ENV PG_SHA256=925751b375cf975bebbe79753fbcb5fe85d7a62abe516d4c56861a6b877dde0d
# Thu, 30 Jan 2020 03:39:48 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:39:49 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:39:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:39:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:39:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:39:50 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:39:51 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:39:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:39:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:39:52 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:39:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1030c456d04636112fa347ddc5296036cddf70c8085be2e3f3fb481898f18fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d0211bbd9a4fd28f739a797600d78394b15d947a30f55f70cfd5daf0f9e443`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59210ffa59a28705da69911cfdcd9e2ead225e06828fd22894e4571259cb8a18`  
		Last Modified: Thu, 30 Jan 2020 03:43:43 GMT  
		Size: 11.6 MB (11551674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938f71a90d4911c2ea572f3724e7b31d9ac746db244c6968b1ecb6bc52d361a1`  
		Last Modified: Thu, 30 Jan 2020 03:43:40 GMT  
		Size: 6.9 KB (6883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74b64391d652dcab5166d1e9fde0c873dcaa78ab8a67c677c05cf74194744b6`  
		Last Modified: Thu, 30 Jan 2020 03:43:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d661539d663b5e1794de5793d6caff610a8013dd018de6995206ec610de99570`  
		Last Modified: Thu, 30 Jan 2020 03:43:40 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e564c2a8119792779de4a4e3ac4cf5d23f8b3014ef2a53b39494a0285312118`  
		Last Modified: Thu, 30 Jan 2020 03:43:40 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5904caabae9a02568af9dec092a210824c2f777a73394e983faf1baff5768e`  
		Last Modified: Thu, 30 Jan 2020 03:43:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:4542ccba8e7e94d93f6f5ae486ac0c03f32e880f13cfccd2f397a7fb65313f30
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13780101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3353e4b9321346c80a3ddbac406560db2d66a4bf180babf669c7399619ac2eb2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:49:35 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:49:36 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:49:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:05:45 GMT
ENV PG_MAJOR=9.5
# Thu, 30 Jan 2020 03:05:46 GMT
ENV PG_VERSION=9.5.20
# Thu, 30 Jan 2020 03:05:47 GMT
ENV PG_SHA256=925751b375cf975bebbe79753fbcb5fe85d7a62abe516d4c56861a6b877dde0d
# Thu, 30 Jan 2020 03:08:17 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:08:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:08:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:08:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:08:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:08:27 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:08:28 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:08:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:08:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:08:31 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:08:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab27e2422be886bc0a338b0e0c20b8e2beea15b880defbac81f75c04495d0c2`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae2520a8d4cdac962b6d4a62335dce896f8ccb0b6d2693b0e72591fda026d14`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bdd0c4de5c351610ae50b6b73c31ec0370f51bfccb3876305a3a473e8f6264`  
		Last Modified: Thu, 30 Jan 2020 03:13:25 GMT  
		Size: 11.1 MB (11149914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a94236ff9ba1418e111dd35663d0b997b1d47cf644f6e24d406570ab281d2ef`  
		Last Modified: Thu, 30 Jan 2020 03:13:19 GMT  
		Size: 6.9 KB (6886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408bedbfefa443f173433ff88eab9e4181687dcb0577769cce0e4ec37444bff3`  
		Last Modified: Thu, 30 Jan 2020 03:13:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bf4620480dc79c692e0f8259d3d6d135f2173e002cdecd69ee85aa1e6aaac5`  
		Last Modified: Thu, 30 Jan 2020 03:13:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17cae6d4ed7b51654876f3215e3e19f36f28f16dc3559ef1b27d6dc3ca3416`  
		Last Modified: Thu, 30 Jan 2020 03:13:19 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8a7644974b357da5359b32efb18da24d5e325a53135dfd99953cd2c1c3ea3b`  
		Last Modified: Thu, 30 Jan 2020 03:13:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:883140df2e1be1a945efe323739225f2cacd0a5f32493f108c7960e6bbe4ad46
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12955729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfd802311ddba7130bf886cbe3baa646541ac1e6c55efe7923a875cdf3ba8b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:00:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:00:13 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:00:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:12:59 GMT
ENV PG_MAJOR=9.5
# Thu, 30 Jan 2020 03:13:00 GMT
ENV PG_VERSION=9.5.20
# Thu, 30 Jan 2020 03:13:00 GMT
ENV PG_SHA256=925751b375cf975bebbe79753fbcb5fe85d7a62abe516d4c56861a6b877dde0d
# Thu, 30 Jan 2020 03:14:58 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:15:00 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:15:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:15:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:15:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:15:05 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:15:05 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:15:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:15:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:15:08 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:15:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572777a7d0992ea05b14f2ba3230ce906c753dd21eb73ac2b6018551250312db`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8810228251d658112d3dbf2b9b1719f402a0c3477bf2eceaa5a20341bba3f5`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59baed7fe8739ffb27042bd819aae7ad863390b032034ea583ea73780ffef88`  
		Last Modified: Thu, 30 Jan 2020 03:20:16 GMT  
		Size: 10.5 MB (10523552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbdbf89b003be8e381b029ed0a8346273d988f7cbb3fb59d315a7814db16147`  
		Last Modified: Thu, 30 Jan 2020 03:20:10 GMT  
		Size: 6.9 KB (6888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9793493bba90a27e9b4800f39617c645f1e6c1a16fe327bcdcb91b0db0a7458`  
		Last Modified: Thu, 30 Jan 2020 03:20:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa6faf3369f94f0976408676ac82053875dda67fbc16010b602e69252920732`  
		Last Modified: Thu, 30 Jan 2020 03:20:10 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f2200f1ec6170253620811293163d9865e51f5eccbe627e7a923c12b0e1c48`  
		Last Modified: Thu, 30 Jan 2020 03:20:10 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dedf28f94930e8c7c4a23ea1008d63d04f76444571130a6153d8e848f87050c`  
		Last Modified: Thu, 30 Jan 2020 03:20:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:f88f15532b01a4c452f7669b4f67685c8193cde790a6c3b8aa96b5a85647bb7e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14127301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17b9c443545042f60e99bf5c516ac3662812a1a82ad42065451f2b7a1222ea34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:40:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:40:28 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:54:08 GMT
ENV PG_MAJOR=9.5
# Thu, 30 Jan 2020 02:54:09 GMT
ENV PG_VERSION=9.5.20
# Thu, 30 Jan 2020 02:54:09 GMT
ENV PG_SHA256=925751b375cf975bebbe79753fbcb5fe85d7a62abe516d4c56861a6b877dde0d
# Thu, 30 Jan 2020 02:56:28 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:56:33 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:56:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:56:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:56:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:56:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:56:38 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:56:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:56:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:56:41 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:56:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db837ff5778a13ace9e439e3bff33c317ecca84803a142a4ee4e05d2af54def`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92b445ab1ef4ba9a6120e5cc359b70cb88b74a46dee803f2709cb873a7be79`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8ec17d0a82f80ed49d26df31dd9e04a2eb396b146eac8586b01a8a40575d67`  
		Last Modified: Thu, 30 Jan 2020 03:01:21 GMT  
		Size: 11.4 MB (11391607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7da858feffa234776a4af82b4b296929c36c34293306fca07c5ba2fcfbeea5`  
		Last Modified: Thu, 30 Jan 2020 03:01:13 GMT  
		Size: 6.9 KB (6885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9da62d0d2bd44cb9ea2b7a26bf42ef6b6132393e940ffecdb0b38398c003ef0`  
		Last Modified: Thu, 30 Jan 2020 03:01:13 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a76e302e72897890480c27ef563860d493ec5225282550822543fb44de307`  
		Last Modified: Thu, 30 Jan 2020 03:01:13 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca1019abc1ecad9bfc252af999ec56d897574ad3370eedc23a5a59f6bd2067a`  
		Last Modified: Thu, 30 Jan 2020 03:01:13 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bfade5cd3ca038731c600f89dbf902fd9f704afa7dc5049e282bcbf80255bf`  
		Last Modified: Thu, 30 Jan 2020 03:01:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; 386

```console
$ docker pull postgres@sha256:b414a43257441d0d7f7ceefe2f8877e6dc3c2e8b1142683ef9cef8eea2aed3fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (14971862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b45ed70d0f364f737c7ca9d8c989b70174e8dcd3f87e4997ab72a0715a40b9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:38:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:38:44 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:38:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:00:01 GMT
ENV PG_MAJOR=9.5
# Thu, 30 Jan 2020 03:00:01 GMT
ENV PG_VERSION=9.5.20
# Thu, 30 Jan 2020 03:00:01 GMT
ENV PG_SHA256=925751b375cf975bebbe79753fbcb5fe85d7a62abe516d4c56861a6b877dde0d
# Thu, 30 Jan 2020 03:03:23 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:03:24 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:03:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:03:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:03:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:03:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:03:26 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:03:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:03:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:03:28 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:03:28 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb8463eb063fd24e3d29bd4ca5b9ba1590717acda7415cb45da3e7560f0dd`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023c33adbfeb9b779f40edac1617b4514e1fb0b976b5b201dd0f7dc688f5e60`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cf17c7cbf2ff19c32ba34492d2b2a019f22d155037c524ad0f8ebb1c2dfcf9`  
		Last Modified: Thu, 30 Jan 2020 03:08:20 GMT  
		Size: 12.2 MB (12152809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6db7d1395a9800546525351b171b1058121811322d9954c3ac565742db40ffe`  
		Last Modified: Thu, 30 Jan 2020 03:08:16 GMT  
		Size: 6.9 KB (6889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a08cae5fe5a4d3c2fcee20cfcfb8ba27f84de2260eec20c94592503db4ebecb`  
		Last Modified: Thu, 30 Jan 2020 03:08:16 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f63a9d597fe6b33859da9d9da06e1af5a94052f7347ca8049f4b319d4323bc`  
		Last Modified: Thu, 30 Jan 2020 03:08:16 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03dea0e8abbd6daaec2e4c1c067b731e86e7f5de3e57e3661b990d2f9021b6e`  
		Last Modified: Thu, 30 Jan 2020 03:08:16 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67db7d3f9d00f159b220cb628a774686c337ac60b81ad41600f2ebbe7e2e06cb`  
		Last Modified: Thu, 30 Jan 2020 03:08:16 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:4cf939d1df0035bc290ba0d1f307e2838235241de661a1eb03385c90e649853c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15271114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:344c936071416c11d0bb64d11d2e4bab42f27fcf8e3bad0460411e87fcdf03c9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:20:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:20:03 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:44:19 GMT
ENV PG_MAJOR=9.5
# Thu, 30 Jan 2020 03:44:20 GMT
ENV PG_VERSION=9.5.20
# Thu, 30 Jan 2020 03:44:22 GMT
ENV PG_SHA256=925751b375cf975bebbe79753fbcb5fe85d7a62abe516d4c56861a6b877dde0d
# Thu, 30 Jan 2020 03:47:03 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:47:11 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:47:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:47:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:47:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:47:30 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:47:31 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:47:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:47:51 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:47:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8af198a4c612619984a3d16dc2a9fb3f15835dfbf5269a9eab9a345ed4f14`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852af7c4759ead6b82b170b6d34d124532026b41ec5d7dc4ec99bd6705f633a`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100d2b17734500a36c69f07b212eebf4b0212450c19eb1e38348f617767de37a`  
		Last Modified: Thu, 30 Jan 2020 03:55:01 GMT  
		Size: 12.4 MB (12436363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d64784a33626dc5f6ad0e55753f24b3a87388441d850628a765b2d6b2e6669`  
		Last Modified: Thu, 30 Jan 2020 03:54:54 GMT  
		Size: 6.9 KB (6886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877b2621d5bb47116ae4adc74e4819ec5c55d39c88bf17d86a10b208ee42029d`  
		Last Modified: Thu, 30 Jan 2020 03:54:54 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68c7a079ae4f258b5a510b9c4047bcdff8eb41e2fdaf31d881aba83bbdeeb8a`  
		Last Modified: Thu, 30 Jan 2020 03:54:54 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4910a4f890c688663d1942a8fbf43c6b273a7a8b943a62b380fa66a739ec3e`  
		Last Modified: Thu, 30 Jan 2020 03:54:54 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13aa1e1072d5b1500f5314274f84ef54265f4ad499144720cf82c10ad6b5d0a`  
		Last Modified: Thu, 30 Jan 2020 03:54:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:95223f78a71fb2a7479dd2914f939acfc37641a40007ddcf24cff6b4f778083b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13965795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ff0d3d57768ce5ef6ca5b5d0916daaa8a94772d05c8bc0beb32e09b29af91e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:48:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:48:56 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:48:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:02:51 GMT
ENV PG_MAJOR=9.5
# Thu, 30 Jan 2020 03:02:51 GMT
ENV PG_VERSION=9.5.20
# Thu, 30 Jan 2020 03:02:52 GMT
ENV PG_SHA256=925751b375cf975bebbe79753fbcb5fe85d7a62abe516d4c56861a6b877dde0d
# Thu, 30 Jan 2020 03:04:35 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:04:36 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:04:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:04:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:04:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:04:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:04:38 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:04:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:04:39 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:04:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d0ab56996305262d42136eee090848bbdf7cec28b8625e39078668b245db48`  
		Last Modified: Thu, 30 Jan 2020 03:07:31 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd3ab8f7e8df3f56e9628a504d2ea6db996a9910565bf84e3bc35bd847bcfb`  
		Last Modified: Thu, 30 Jan 2020 03:07:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2453418375b13c27f7c0bd946bdb80c5dc40ef671797bf1858731773b9bbd7`  
		Last Modified: Thu, 30 Jan 2020 03:08:33 GMT  
		Size: 11.4 MB (11371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10295071e4cf2c94d583b8af503a058a9bbb5ce65e43dcc54ec3c81cae6a8e9e`  
		Last Modified: Thu, 30 Jan 2020 03:08:30 GMT  
		Size: 6.9 KB (6880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49e920ee78b6ced90be6c80b1507fc8dcc0ca5652ff04ccfdfe7010428acbb3`  
		Last Modified: Thu, 30 Jan 2020 03:08:35 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccbca11c51c0f958387e54369aad406cb39c12a144d28dee4b3df532b7f5f17`  
		Last Modified: Thu, 30 Jan 2020 03:08:30 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd33a500897207e19d92e03e53ea29c152f5ae1f32828fa0f2403050fcff4e74`  
		Last Modified: Thu, 30 Jan 2020 03:08:30 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063006c47158b6fca7dd710c1b8c3724f8a0a6fb403822675e9662ee56e0b370`  
		Last Modified: Thu, 30 Jan 2020 03:08:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.6`

```console
$ docker pull postgres@sha256:d6a6badb2b5b22de5e135490a217522cecc2ae90fe35b33290615827569310a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:9.6` - linux; amd64

```console
$ docker pull postgres@sha256:c5df9349b2a361769ea3859d9d6b675cc3c08aab564115ab936632447aed15be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.0 MB (87992167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb2889ab0680ba518e0dc1bb5a09cbe23f1e5908d9e484daea3d34f5e092ec17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:23:57 GMT
ADD file:003d2bac85e72555ed93f77a2b1d595a7fe51c4a9a2401496a82fc673a863fd6 in / 
# Sat, 01 Feb 2020 17:23:58 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:07:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 06:07:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 06:07:31 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 06:07:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 06:07:59 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 06:08:00 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 06:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:08:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 06:08:12 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 06:09:45 GMT
ENV PG_MAJOR=9.6
# Sun, 02 Feb 2020 06:09:45 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sun, 02 Feb 2020 06:10:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 06:10:10 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 06:10:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 06:10:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sun, 02 Feb 2020 06:10:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 06:10:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 06:10:13 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 06:10:13 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:10:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 06:10:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:10:14 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 06:10:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:619014d83c026bca3d21f5eb42a629ac2dbe15bdb37b77f25fc1ac5fbada68e5`  
		Last Modified: Sat, 01 Feb 2020 17:29:01 GMT  
		Size: 22.5 MB (22524713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec0fe6664f6bb5f06d5d0a9a68c99a68be052403c684a8ffd98e70f6256d8ca`  
		Last Modified: Sun, 02 Feb 2020 06:12:59 GMT  
		Size: 4.5 MB (4501301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7ba8f77640450af762ebf643f368663949425d1bd516521dd9c0022a65461`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 1.8 KB (1779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1155d037e2c8553fc58b2671c2e61ca9ee29c7f712dbfc66dc20e8ab549c6b`  
		Last Modified: Sun, 02 Feb 2020 06:12:58 GMT  
		Size: 1.4 MB (1351457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febcfb7f8870017ab69faa0a454aa6a1e3cfde53c46074d1aa3e6edaea01adcc`  
		Last Modified: Sun, 02 Feb 2020 06:12:57 GMT  
		Size: 6.2 MB (6182941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c78c79412b5cb255309e404e829646cc509a10cf8f55b2a5043da04d706604c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 295.6 KB (295582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a35744405c5f473d3002c5451970e6ff78bcc5eb330eea1c5595cca6b32679e`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27717922e0679badf783f2aa3179d254bb023533caf48d859c3d29723401701c`  
		Last Modified: Sun, 02 Feb 2020 06:12:56 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577de7c4ffdc4243fbaee8f228488837f2f9a2f2c87a68202abaea93ded28b88`  
		Last Modified: Sun, 02 Feb 2020 06:14:00 GMT  
		Size: 53.1 MB (53117400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3482e27d98ae9056b29a5cdd582dadcb8ca915fcd335fb73b061a85e50b6f8`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 7.8 KB (7823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ff898274ac109dcef4fcfa92b07409953f2f4363ecd0d73cc0b004f00f0815`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6131782ee224b1daac69e6d7f6b38b744422334fb5906b6432e929c3d32782`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496ebd477eeafd1b47febb4fc082afafd21079521d1b93c519265d5bcbe0e414`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f0da1de185b12370cf4623340f2058fa5a2a3560fd926d0e8b07f6fa22cb30`  
		Last Modified: Sun, 02 Feb 2020 06:13:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; arm variant v5

```console
$ docker pull postgres@sha256:156b34423cbba4d94ba6cdad7d3f45648230879051597dca3222c8a8f87c0245
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84491279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9103688e54d3b96fec8326d286a3bb0a3680ab194f4a7ec614c89051b989eb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:53:57 GMT
ADD file:f0d179649cbf50028b5ecd832961cc332fb524c2f12fda6c8060c3c258208be6 in / 
# Sat, 01 Feb 2020 16:53:59 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 19:04:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 19:04:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 19:04:31 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 19:04:59 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 19:05:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 19:05:16 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 19:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 19:05:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 19:05:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 19:49:02 GMT
ENV PG_MAJOR=9.6
# Sat, 01 Feb 2020 19:49:02 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sat, 01 Feb 2020 20:09:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 20:09:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 20:09:20 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 20:09:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sat, 01 Feb 2020 20:09:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 20:09:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 20:09:27 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 20:09:28 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 20:09:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 20:09:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 20:09:32 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 20:09:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:03886a8604d1b5423798ee97917dcb9de4cfdfbb7c435a7988d5c5e69a78e3b7`  
		Last Modified: Sat, 01 Feb 2020 17:01:03 GMT  
		Size: 21.2 MB (21202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aaa01ea1502b56b5ebd804228ff2ea5ad2adf78d4797d7a6aa75903a7dc7a30`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 4.2 MB (4236888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feeb9ed754ebd60d2d8cdffa636ff7e5b6ea1b1f68fd7c7aac5f1dced2f8cf9`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142683156b4ad1e2209ecaac30f55cd1a7237fe046f545e7a64613b34c221671`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 1.3 MB (1311293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950d1d965477d4d1230281bd3043f7347d94e263cada82cd86f3f055cc269e93`  
		Last Modified: Sat, 01 Feb 2020 20:51:02 GMT  
		Size: 6.2 MB (6185421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1690d5dc7daff0def912cfa3c22eff87c80edb8f734454280c116e5fd52ebb92`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 293.5 KB (293479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0191375b3084722e33f875137d737673fc3ec09776716614c4fcd6764e7884e`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9bf11db5cc7dd3ff01824ff16d5642657294a22e3ec2086a5b3575ef803947`  
		Last Modified: Sat, 01 Feb 2020 20:50:59 GMT  
		Size: 4.8 KB (4791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0243666d93d53a13ddedd28e800d1c27f6d6a89faabb40345177bec3ad01664b`  
		Last Modified: Sat, 01 Feb 2020 20:52:15 GMT  
		Size: 51.2 MB (51242498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a8b7d0740023a25af9ac759b731a38892cd1b4944e18d5790549e52203ee4e`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 7.8 KB (7822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d17cd9d8d74696e07f0eb85d3232d957faf2db274d18f0d7c53043b786834`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724495e2c1ced93f7ae7635b5653dd7d82256e8726814b76e32668732e9a2432`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fa4ca3b32534986ebdb3e5a073f4478ed6e34bec824033f13822a3313dd03c`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5708c0cab5dc7637b4e00100d14dc31ef6438188a0d43fdadfb1cda8e9b49087`  
		Last Modified: Sat, 01 Feb 2020 20:51:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; arm variant v7

```console
$ docker pull postgres@sha256:6176db12c5cd603cf2deeb0ece0c394a94a0b491f5b34418adf90bb2959118bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80638829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df1d2a74bab23c4cc256ff5e5f7a91965712471e65e31155b72fe23970346cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:04:29 GMT
ADD file:6ac430a42a1f2a6cc8b0a3565e518bd0e3a47b01d524b86cd3dd4e7f4606fd53 in / 
# Sat, 01 Feb 2020 17:04:31 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 08:58:06 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 08:58:07 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 08:58:30 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 08:58:44 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 08:58:45 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 08:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:58:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 08:59:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 09:40:04 GMT
ENV PG_MAJOR=9.6
# Sun, 02 Feb 2020 09:40:05 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sun, 02 Feb 2020 09:59:01 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 09:59:08 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 09:59:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 09:59:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sun, 02 Feb 2020 09:59:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 09:59:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 09:59:17 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 09:59:18 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 09:59:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 09:59:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:59:23 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 09:59:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6bc458b0813423b9e351a5604c0d71a4853d970ea22b23fedc8683af12dbc13c`  
		Last Modified: Sat, 01 Feb 2020 17:11:31 GMT  
		Size: 19.3 MB (19311624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e359f7642afed089b2d05ece4e0736e03ceb13a937f7478eb868702665f809`  
		Last Modified: Sun, 02 Feb 2020 10:36:41 GMT  
		Size: 3.9 MB (3872826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7b5742cb7fbb2cdb38f99c354efd420d24d27dee9b21b232dc92100066c10b`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6852094413bd98c461152c87837e91176b94a6cadae25e1a31b7f07330ecc4`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 1.3 MB (1303620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589bd77312350a872d2ebc5a6638ec844bf3aece0160a35b34a5d5cf66ae0d22`  
		Last Modified: Sun, 02 Feb 2020 10:36:40 GMT  
		Size: 6.2 MB (6185708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943e832035ee98c3689f148b48e73550099b8f81fe37da09aa6e1ae2ea1756ac`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 291.9 KB (291867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba8ac21d907e788e2f05af094077cd10bcd20b8bb6eb5021b9f01ae1cfb1d97`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f8d5c6112a73a87453a9f3b2c2c298c0d2c275026fb63fb5ecdd81e6205461`  
		Last Modified: Sun, 02 Feb 2020 10:36:38 GMT  
		Size: 4.8 KB (4792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ea67ee1c6fb5d3075dbf0b963e7d7689e2393a836c4a3b3065195103a393c3`  
		Last Modified: Sun, 02 Feb 2020 10:37:51 GMT  
		Size: 49.7 MB (49654325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc7ea1bf1b3ba1ffea659c5edb02dc3dc37ca858be0093a87bb3098bb6e6315`  
		Last Modified: Sun, 02 Feb 2020 10:37:31 GMT  
		Size: 7.8 KB (7819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1591631eb0d69c23e4d2116eeadb0aec1ae49bbf686e3c1cc9829847b19cc5e5`  
		Last Modified: Sun, 02 Feb 2020 10:37:31 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e59bda490195f44526b0ff46921e8c3216469ee27448053793917ecaf4561df`  
		Last Modified: Sun, 02 Feb 2020 10:37:31 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd73775a0650bd8db6494735b191ee5b9a411883de6a7e25058138a7af0ca60`  
		Last Modified: Sun, 02 Feb 2020 10:37:31 GMT  
		Size: 3.8 KB (3846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bd23b1945cdfbfdc79db97f4aa956fd8f7ba1affe7121cb367da74b4bf8ae3`  
		Last Modified: Sun, 02 Feb 2020 10:37:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:3fbc177c71c33002547b77433ed04c2f54964c582ea43ef9d25c4edb94d87366
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.5 MB (83499997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9706bc1df961358808bfd77c775181ec51651ad54e6cb57fc25f9b6381ad04a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:19 GMT
ADD file:d3338eed8ee88c2a5856cc2eb73701e4de79a7e551602df07834a1ad4f671435 in / 
# Sat, 01 Feb 2020 16:43:21 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:24:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 02:24:24 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 02:24:27 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 02:24:52 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 02:25:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 02:25:09 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 02:25:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:25:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 02:25:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 03:08:47 GMT
ENV PG_MAJOR=9.6
# Sun, 02 Feb 2020 03:08:48 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sun, 02 Feb 2020 03:28:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 03:28:27 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 03:28:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 03:28:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sun, 02 Feb 2020 03:28:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 03:28:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 03:28:35 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 03:28:36 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sun, 02 Feb 2020 03:28:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 03:28:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:28:42 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 03:28:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5c630fa6465ea72ddec15fd68bdd45a6da6fa4b1981895bf7c2852eedf066194`  
		Last Modified: Sat, 01 Feb 2020 16:48:58 GMT  
		Size: 20.4 MB (20385851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a29899232ff5984832260695109c206ed14783ab8a33dd8f593f40672e2cf51`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 4.1 MB (4077687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72390476b7ab26db4e6e224ad16f9c0a3d66dce6b4d9996f6edece0992dec78e`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f4470eb370695bb8691186ee389e7be5deaeb4f0d84a84ca948ae39ea977a1`  
		Last Modified: Sun, 02 Feb 2020 04:07:21 GMT  
		Size: 1.3 MB (1286440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b51db6dc34b50eff6b5d8120f3efff4e5269216d5ea5d004ce80782e7508411`  
		Last Modified: Sun, 02 Feb 2020 04:07:23 GMT  
		Size: 6.2 MB (6185392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918217c35d15c52bb58861e8c65a6b6934bc554387043c67b630758273c41028`  
		Last Modified: Sun, 02 Feb 2020 04:07:20 GMT  
		Size: 292.1 KB (292139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea01905f4f686b651e994714cb840779b241fcf43c04c6cc2a0ae229543862dc`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ff0687a25d7e24b75be4e353f57d8821a81a4b8c51aff2a01f927bb70d1a76`  
		Last Modified: Sun, 02 Feb 2020 04:07:19 GMT  
		Size: 4.8 KB (4794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9424f08e065d6d18e3d2b4ce50ddede234d07b7cd7f54aa614eb5d92a1862ce8`  
		Last Modified: Sun, 02 Feb 2020 04:08:28 GMT  
		Size: 51.3 MB (51253618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b912d4a038fb1bbb67af442be67dd04e068043b1f07167149b5dc1bab352b9`  
		Last Modified: Sun, 02 Feb 2020 04:08:09 GMT  
		Size: 7.8 KB (7819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2539c3f1d8eef8f0f55c2471f0896f3e7448e6fefea11731b315999ab35dee`  
		Last Modified: Sun, 02 Feb 2020 04:08:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02a4185c7f2fe75b83ce98818c61040b6066de3db6eabcb5dc3c56d80ea411`  
		Last Modified: Sun, 02 Feb 2020 04:08:09 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae02c764537af80292160bf0c69b4137d6163ccea411bd4ce93f4dc0e10790b`  
		Last Modified: Sun, 02 Feb 2020 04:08:09 GMT  
		Size: 3.8 KB (3848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94f68ec254f3c01c9811f77eab5b38bcbc19f18cdb79a16bc9dde24b20d71dd`  
		Last Modified: Sun, 02 Feb 2020 04:08:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; 386

```console
$ docker pull postgres@sha256:0cc60c7ca6aa2b656d5be080630da5245a1d25547e5d531580ce826d789e165d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89369641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b07066394842fba9794666320ff1073131f9849b1e76bb494969683718fa1b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:07 GMT
ADD file:c9b4696be461d46d96c760441f34e219e229f90bc6946125b2f809218c3456ce in / 
# Sat, 01 Feb 2020 16:42:07 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:21:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:21:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:21:11 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:21:27 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:21:39 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:21:39 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:21:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:21:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:21:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:24:05 GMT
ENV PG_MAJOR=9.6
# Sat, 01 Feb 2020 21:24:06 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sat, 01 Feb 2020 21:24:47 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:24:49 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:24:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:24:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sat, 01 Feb 2020 21:24:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:24:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:24:52 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:24:53 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:24:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:24:55 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:24:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4f51b031b74b1f7fab6310c197fd7534181ba2db1f0cec6686fb9e9a82abbb9c`  
		Last Modified: Sat, 01 Feb 2020 16:47:27 GMT  
		Size: 23.2 MB (23152156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400715a0cf80a4163f9bdfb01029e10c149b8ff3ce6ef1248f400451f617b081`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 4.8 MB (4807817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57223b59a38681596adf27043fcaa0c4896293e4b8d488d81957c76d11ee0d7`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb13941b5f12a8251a7c85981cb0d44069be9f4d1644bc34a11ae761968abdd8`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 1.3 MB (1318016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ada6bc6e6f24824fc92e6f96abb0ec680d29443a640d4b03d2ac54a6cb74ba`  
		Last Modified: Sat, 01 Feb 2020 21:27:37 GMT  
		Size: 6.2 MB (6182955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65761eaa1a3239dc440a674c9a27612170189ab04f41d5360678cc34ddfab827`  
		Last Modified: Sat, 01 Feb 2020 21:27:33 GMT  
		Size: 296.8 KB (296752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81305139d5a6d74e0ed5bf9ba0163f5c6baf0c66890f74d05e94b5313a57d86e`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ff425a04fcdc853777162926c616c569257ea00e96154204e9e3f91e2f7527`  
		Last Modified: Sat, 01 Feb 2020 21:27:32 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa669fa7d13b33dbd17a9edc07645f1d8055817b4fca8ab2ce671f36d9c9fca8`  
		Last Modified: Sat, 01 Feb 2020 21:29:09 GMT  
		Size: 53.6 MB (53593187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018e1562dfbad2ab7b61a76e7ba8fae2df8289ec6bfefc5f33b450c6a382bea5`  
		Last Modified: Sat, 01 Feb 2020 21:28:45 GMT  
		Size: 7.8 KB (7817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a85f32c119e7b1840ce73e2514c57b808d291dbb573a8e25bf5e8272f7669d`  
		Last Modified: Sat, 01 Feb 2020 21:28:45 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36872fb92973a9d1aef694535a04ea9e87f661d5e378927dc6c3b4922f790c8`  
		Last Modified: Sat, 01 Feb 2020 21:28:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e02424a08286578a82a1c2ca3e657020c6d852022f3c62a2a705dc9ba91f60b`  
		Last Modified: Sat, 01 Feb 2020 21:28:44 GMT  
		Size: 3.8 KB (3844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82941b4e2b391ceb761d3d6f6d27b8569dc2a9ee4a35a24c0cf62c085eaeaaa`  
		Last Modified: Sat, 01 Feb 2020 21:28:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; ppc64le

```console
$ docker pull postgres@sha256:78828c61f1b443c1ada7ffaf07ccd43d6cbcc1ab539d2e27862920106ec4b856
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87711767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6f614dda0c03db1138211867f66644c057e66e8171997d60481600b17119483`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:8840e8b11ab671d52cc308dfcd68117cbff88d7e5e18e0628683d75699a7c131 in / 
# Sat, 01 Feb 2020 17:20:49 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:34:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 22:34:47 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 22:34:48 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 22:35:35 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 22:35:55 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 22:35:58 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 22:36:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:36:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 22:36:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:45:00 GMT
ENV PG_MAJOR=9.6
# Sat, 01 Feb 2020 22:45:02 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sat, 01 Feb 2020 22:47:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:47:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:48:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:48:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sat, 01 Feb 2020 22:48:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:48:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:48:17 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:48:18 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:48:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:48:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:48:29 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:48:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4b12198d119cc40a2102fa8f986f1f3bc6f22967a421939f96b52470129050b9`  
		Last Modified: Sat, 01 Feb 2020 17:31:15 GMT  
		Size: 22.8 MB (22800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760805deb1a123f70f866680db67bfa3dcb8847b6ba0a19aa81db56e389e2fc0`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 4.4 MB (4364947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07edca5c09c7a639b08f5873160d9f51a67dca693c553c77bd4da3a487cf98b1`  
		Last Modified: Sat, 01 Feb 2020 22:57:59 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531ca140aa96954bbf71328b29b544b3a2e6d65750bde462ebaf5ceb9211a2f3`  
		Last Modified: Sat, 01 Feb 2020 22:58:00 GMT  
		Size: 1.3 MB (1274917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5387f07d48aa567c90a5f600a88d52a3e23731fc526fe455615270e71eb87826`  
		Last Modified: Sat, 01 Feb 2020 22:57:57 GMT  
		Size: 6.2 MB (6185756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df00257572bca93ee8879d856b2ad35f675ee82aa6091ca73d467ca3743f67ed`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 293.5 KB (293536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d078612d1275942888b21d29cab572493f1e313c54b050434dcd70e2d76d544`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2e5ca1d60f37146aeff96ecb4c62cbe26cf5ebc72cb162751de46927921192`  
		Last Modified: Sat, 01 Feb 2020 22:57:55 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0002035012ee6890ccde192d4b8382739b92a74d7c85020963046efc6c5bcd17`  
		Last Modified: Sat, 01 Feb 2020 22:59:06 GMT  
		Size: 52.8 MB (52772968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46e454b022b67067d2501e2bf6e71e8026a96ce04ec0188a00c5b5be5855fa4`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 7.8 KB (7833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50e5ae5b23eb887386d3d0d1902a9c59f0f7188a1a9f60a8d6856c4c0fc16d8`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f879a88c785812c8459cb56b4e86361265724a90985bf2f3550602a04c300bb6`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c088fbc21c50d68a5735d71d1d46b17da2caf2178d8b9670fdebd525d5d17117`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 3.8 KB (3845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9451f99ea65c745ef67c24042b50919eae46e00b0841446566dee9fed0d365f8`  
		Last Modified: Sat, 01 Feb 2020 22:58:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; s390x

```console
$ docker pull postgres@sha256:4c6b34f3acfccb569d33132e5ad4479fdc089a26d798c424ede97d837d77932a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.3 MB (88297071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad50f8eb12b75d3c44dcc6af7f32ad5f92dc07b05847933aa1e9ee5c9774bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:43:55 GMT
ADD file:cf4bb119f25d8a9b9a2cd43101d5e87e0dbaa42d3f6688b39e66eea637225cc2 in / 
# Sat, 01 Feb 2020 16:43:57 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:40:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:40:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:40:14 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:40:23 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:40:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:40:28 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:40:32 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:40:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:55:32 GMT
ENV PG_MAJOR=9.6
# Sat, 01 Feb 2020 21:55:33 GMT
ENV PG_VERSION=9.6.16-1.pgdg90+1
# Sat, 01 Feb 2020 22:02:08 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:02:11 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:02:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:02:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sat, 01 Feb 2020 22:02:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:02:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:02:13 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:02:13 GMT
COPY file:cbee5ff17d821d73b1907a597065e0b50774f8971d6495e6d3792ca01d557a2c in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:02:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:02:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:02:14 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:02:15 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:24a7c24214752593c0f651c56554e1bc6056ce340eb46cb71ed7ff0c430845a8`  
		Last Modified: Sat, 01 Feb 2020 16:47:44 GMT  
		Size: 22.4 MB (22380184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba584ff8c21579486e3687e8a4f6d0ecc911f32353708e9693752a64526d34f8`  
		Last Modified: Sat, 01 Feb 2020 22:15:15 GMT  
		Size: 4.5 MB (4534611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437afaa09e73336a77de2eaf796fdf66bd35380394ac42d0840b500f8a4972df`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1625730f985442686e8bba703b5a2f74d8ebb56b6c3f09d255ee5520ae0b83a`  
		Last Modified: Sat, 01 Feb 2020 22:15:12 GMT  
		Size: 1.3 MB (1340980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505f199fff79fe4eb15264a3e92774fffb954fa9ca0b399800fafb2991aba6ea`  
		Last Modified: Sat, 01 Feb 2020 22:15:13 GMT  
		Size: 6.2 MB (6209613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea830cdc46d22c2ae31a6b440834f2563d2e28b2548c24b1daac41d82482f5f4`  
		Last Modified: Sat, 01 Feb 2020 22:15:11 GMT  
		Size: 294.6 KB (294550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c761a50d986b42286d1616f6bb992a8469b97207f4b48e434a5b6a81e2fe6`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc1bb55d92f21306a95cb3259eec2a3f3659245aeebb728d6698b7be3381b8`  
		Last Modified: Sat, 01 Feb 2020 22:15:10 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54701b00a2872abeaf7e53c507b139529edc55392fb9fd1e730faf75bb833e2f`  
		Last Modified: Sat, 01 Feb 2020 22:16:13 GMT  
		Size: 53.5 MB (53518265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4e19a6f21d1cbb059a3eb3396945ebb64445c7acec95f0a20fd2a279068114`  
		Last Modified: Sat, 01 Feb 2020 22:16:03 GMT  
		Size: 7.8 KB (7819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e850dc1856bbd7bf63f47d449e8419ddc3e1da8fd9d3ccdea56cf30613fd42`  
		Last Modified: Sat, 01 Feb 2020 22:16:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375da53893bc523d68007c4526135647aefbac3618bc070b81abeed42a188921`  
		Last Modified: Sat, 01 Feb 2020 22:16:34 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f59d9757749cc559a6c6075fe6d6e5ed5a0c4f85094ef695cc153b7bddd2f8`  
		Last Modified: Sat, 01 Feb 2020 22:16:34 GMT  
		Size: 3.8 KB (3847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c09fda018d62ac9c322bee2a8ed2ee56e56f5b5780d6e43e669678efc414be`  
		Last Modified: Sat, 01 Feb 2020 22:16:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.6.17`

**does not exist** (yet?)

## `postgres:9.6.17-alpine`

**does not exist** (yet?)

## `postgres:9.6-alpine`

```console
$ docker pull postgres@sha256:8ec15b51fd1ec3233ca7bcf3a58e800d863f57c8d07ffdc65fe4640a19f7b2e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:9.6-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:3a1d32d67fff9d004a8fb50cbb4c7854dca176a9624ea12ba1bb9a5321e8eac1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14649269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d8fbe8dd6b511590196d244e0771e1f010eb96833adf3b3215417adccc8168`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:19:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:19:59 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:34:11 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 03:34:11 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 03:34:11 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:36:51 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:36:51 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:36:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:36:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:36:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:36:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:36:54 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:36:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:36:55 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:36:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1030c456d04636112fa347ddc5296036cddf70c8085be2e3f3fb481898f18fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d0211bbd9a4fd28f739a797600d78394b15d947a30f55f70cfd5daf0f9e443`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1057c9a28776b9ab60a6a0a79afb37a5d68f1ec650c9c1a1e95a5e161d023c6`  
		Last Modified: Thu, 30 Jan 2020 03:43:35 GMT  
		Size: 11.8 MB (11833542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc0c32069403f3e0a4f55c207150573a3bb394b724b76dafdd8047fc23b5df3`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ae0e20a91aabdf806c18dbdd7d9fa57ff9451d8354fe67ceee55d856261711`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52891a1e287134685d008b61d9c2d00b7221a3e7bf5a538ee8d598dbab98415b`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade8b42d5008d85cee916e695a1da705b04a744722172eaabe685ec30c71382`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedc566e2fda6435ca2aaff8334c3690c8463e77cabfe275cc70ff7046f65686`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:661bd96681eb4625bc7fba9559b8920adfb41f14e3ee51075f2b3190f6f136c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14040955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a667f9e70361ee42baff053b3ce63b6a84f42d24ba2055dc63ce2be52afc4047`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:49:35 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:49:36 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:49:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:02:30 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 03:02:31 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 03:02:33 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:05:14 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:05:17 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:05:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:05:20 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:05:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:05:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:05:23 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:05:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:05:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:05:30 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:05:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab27e2422be886bc0a338b0e0c20b8e2beea15b880defbac81f75c04495d0c2`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae2520a8d4cdac962b6d4a62335dce896f8ccb0b6d2693b0e72591fda026d14`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6dda155ab6da3f7ce5a0a095b31f550ad1eec7400f992ce356739d2cc13322a`  
		Last Modified: Thu, 30 Jan 2020 03:13:11 GMT  
		Size: 11.4 MB (11410503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fdb21a7a829d858ac12aa032091ca59612507b5c90725646c5d65e2cc94e7b`  
		Last Modified: Thu, 30 Jan 2020 03:13:02 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35936da04d6e44ec4b999a8e2fd12bcd4005d87a9eb96247c6ba7e901b7593`  
		Last Modified: Thu, 30 Jan 2020 03:13:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cbc4d887b3f8ca246d14d7e7e74ad0fd37bdee30947d7c4476f44eed62cb6c`  
		Last Modified: Thu, 30 Jan 2020 03:13:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a449e0683710f8a1fc54b307dc9d12f86cc429d2e5dc3e172aa97d091612d6fe`  
		Last Modified: Thu, 30 Jan 2020 03:13:03 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed69b99af5471a2076c49109a08a03a3cf60bd9e4f6a7cb33f8914b3face753a`  
		Last Modified: Thu, 30 Jan 2020 03:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:539d79e1ab79b18f4aa35f9c3a393582b7a571fccbb817b66e9f6f243d679fc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13210081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dee6416c8a156bc2a95d3dcbb4a01c07243238e50687f792a1b2f7260ca9c7c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:00:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:00:13 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:00:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:10:24 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 03:10:25 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 03:10:25 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:12:30 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:12:33 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:12:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:12:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:12:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:12:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:12:39 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:12:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:12:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:12:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:12:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572777a7d0992ea05b14f2ba3230ce906c753dd21eb73ac2b6018551250312db`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8810228251d658112d3dbf2b9b1719f402a0c3477bf2eceaa5a20341bba3f5`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4a4696e10febf1192fc41774e4996a9c99fab6cc6dd148f2c7e2baccb3d4c8`  
		Last Modified: Thu, 30 Jan 2020 03:20:02 GMT  
		Size: 10.8 MB (10777629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5dc0ebb7e5bcfad548b278494935b59ef68bb175ee5269bd651ac11b6165b9`  
		Last Modified: Thu, 30 Jan 2020 03:19:57 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fac1cf77ead444c3aae0b40bad245e46b67485edcb28fc5e68ca82ca5c20e`  
		Last Modified: Thu, 30 Jan 2020 03:19:56 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44def7b6fb7128bd73a57749b60c6494934f44a032a5853f4b33c8a7287272e3`  
		Last Modified: Thu, 30 Jan 2020 03:19:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11acc24b73cf50d5a7dfb16a359dcb3952f255a2c993b5cacfd45b093986e2d`  
		Last Modified: Thu, 30 Jan 2020 03:19:57 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a650ba71db65a089810172ab8b952fbffc483232cc4504228baa2e9c08712`  
		Last Modified: Thu, 30 Jan 2020 03:19:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:07e2b0c89d90a2656c012fd06b9f167ce78b02e5631aae0f06123354d4d119eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14413467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b984aa4f7ce2832012a15d76412facf070ed72cd310854291891c125daa07986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:40:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:40:28 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:50:49 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 02:50:50 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 02:50:52 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 02:53:26 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:53:28 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:53:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:53:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:53:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:53:40 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:53:40 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:53:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:53:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:53:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db837ff5778a13ace9e439e3bff33c317ecca84803a142a4ee4e05d2af54def`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92b445ab1ef4ba9a6120e5cc359b70cb88b74a46dee803f2709cb873a7be79`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c972a35f031edcc5519cb2d82fd3e75925c0f166bcc51cf07b5d0f6d6520ba98`  
		Last Modified: Thu, 30 Jan 2020 03:01:02 GMT  
		Size: 11.7 MB (11677499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e156b311e59e67533aa89c29ebbbf0010a90dfe599a91e461be03237bea41a28`  
		Last Modified: Thu, 30 Jan 2020 03:00:57 GMT  
		Size: 7.2 KB (7155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d8d5c59fcd5ec94c54bf9f2d43324ae4af5c52449b00a6340aa550fa1130e`  
		Last Modified: Thu, 30 Jan 2020 03:00:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e176c5ad16776b3ed9c78a826c56b6805805ea6c7de3dc1a6d9399cb77fa290`  
		Last Modified: Thu, 30 Jan 2020 03:00:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77b47d2704d263cad4b8f1e90c58d1d16d6227924428a9bdd1bdbf3cfeeeadc`  
		Last Modified: Thu, 30 Jan 2020 03:00:57 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a42e1479a8b7c8101baaa134ee430b65e5b52f4983a7624f61ca9224d0cb7c`  
		Last Modified: Thu, 30 Jan 2020 03:00:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; 386

```console
$ docker pull postgres@sha256:212041f986e8c8756149494defae89b95c815bfb0c152df58b975706ba4acb90
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15275660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0080c1225896c0760aefebf89f0b0664bcd8c29cdae559322541cea73b49e60d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:38:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:38:44 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:38:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:56:13 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 02:56:13 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 02:56:13 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 02:59:42 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:59:43 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:59:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:59:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:59:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:59:45 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:59:45 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:59:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:59:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:59:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:59:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb8463eb063fd24e3d29bd4ca5b9ba1590717acda7415cb45da3e7560f0dd`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023c33adbfeb9b779f40edac1617b4514e1fb0b976b5b201dd0f7dc688f5e60`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49f93678df794c61a1d72144fb23535044c306682a96aa160c18349e111b0a`  
		Last Modified: Thu, 30 Jan 2020 03:08:11 GMT  
		Size: 12.5 MB (12456337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b2cc2c8a06f7a47991da929b764b8d671a4080d9b01564fa8f7cd5007fdd7e`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 7.2 KB (7155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c720332a64317c5d72a640d63a9ac0b5762b9af6db25c51a53983c941f0861`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492617946eec1c296943b7dcd1d7940fb689d1b19b22aae530eeacf948352ef8`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a106bf288ba4d1ce2a3dd80535b186dc29df23524b0dbdc496b9026bf552c0`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1436738e877347996a2bf14590058d8173fbbf89605b47946030c9ad24f934`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:928d7215380bbe77f4962bd9fefcfafd1e93e943b1a8293bb7808acce94499f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15557345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd7d92f86da623a8f2596cd1856ff14fbfa66184df49c00e77f6a7d7c3ef2c0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:20:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:20:03 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:40:19 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 03:40:22 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 03:40:27 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:43:14 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:43:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:43:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:43:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:43:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:43:40 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:43:41 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:43:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:43:59 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:44:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8af198a4c612619984a3d16dc2a9fb3f15835dfbf5269a9eab9a345ed4f14`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852af7c4759ead6b82b170b6d34d124532026b41ec5d7dc4ec99bd6705f633a`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658b58d94cab97c61d02b3a48350135284a608d0320139f7a5eee377c6243940`  
		Last Modified: Thu, 30 Jan 2020 03:54:41 GMT  
		Size: 12.7 MB (12722332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e35da3fdb3ab1ade3aef76ad7731b086f053589265905231456f7a1a3567b6`  
		Last Modified: Thu, 30 Jan 2020 03:54:34 GMT  
		Size: 7.2 KB (7153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610b71464c957c7cf7b312c32eb52c09d253138140ccea9ffa89349241933432`  
		Last Modified: Thu, 30 Jan 2020 03:54:35 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5add389f209669a388abb071108374100f053ce522b5774e1a1a0ecee1070f`  
		Last Modified: Thu, 30 Jan 2020 03:54:34 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d755d4533dbc318ffbb92b60488a2d0b77189f2f1040464217be65a9e40716c`  
		Last Modified: Thu, 30 Jan 2020 03:54:34 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4724b9087057f88efec97eb8bfd895b60bb8be28e19551d148bc87a0c96083`  
		Last Modified: Thu, 30 Jan 2020 03:54:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:7ec9d24814d44d459ec11cd58447428622859319979c3af4476e7346d385d7ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14249101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93326dfe2430e3ba3d2bd4878844bbc7b291b017f7c097e625bcf6e3c50fe2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:48:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:48:56 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:48:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:59:45 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 02:59:45 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 02:59:45 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:02:34 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:02:35 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:02:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:02:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:02:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:02:37 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:02:37 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:02:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:02:38 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:02:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d0ab56996305262d42136eee090848bbdf7cec28b8625e39078668b245db48`  
		Last Modified: Thu, 30 Jan 2020 03:07:31 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd3ab8f7e8df3f56e9628a504d2ea6db996a9910565bf84e3bc35bd847bcfb`  
		Last Modified: Thu, 30 Jan 2020 03:07:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a126ed3287b34fe720c506263021e7e31a184968e7ff47b009d604aa72ad689`  
		Last Modified: Thu, 30 Jan 2020 03:08:23 GMT  
		Size: 11.7 MB (11654177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c64d812928562f857ddf834ec04f744e6003fab53071d9467debe4c5b5c4`  
		Last Modified: Thu, 30 Jan 2020 03:08:19 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45928fc7ce5df2ca490cd83d3b0913dd5c32a6f2b1a2d455c30b094bca7b555a`  
		Last Modified: Thu, 30 Jan 2020 03:08:24 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538d02a45edb1fc3ec2260fe2fab21efb3b212ea7ee5f94977c5876a845368d0`  
		Last Modified: Thu, 30 Jan 2020 03:08:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4df51723193fea68bd8c8f608c1a8fafa9818e3006e1eb2d8e8993485db490b`  
		Last Modified: Thu, 30 Jan 2020 03:08:24 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724156134ac6ffb3e96504c647e1f00d5d6d02bbf8f812d98a683f4c28c8ebf2`  
		Last Modified: Thu, 30 Jan 2020 03:08:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:8ec15b51fd1ec3233ca7bcf3a58e800d863f57c8d07ffdc65fe4640a19f7b2e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:9-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:3a1d32d67fff9d004a8fb50cbb4c7854dca176a9624ea12ba1bb9a5321e8eac1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14649269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d8fbe8dd6b511590196d244e0771e1f010eb96833adf3b3215417adccc8168`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:19:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:19:59 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:34:11 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 03:34:11 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 03:34:11 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:36:51 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:36:51 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:36:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:36:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:36:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:36:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:36:54 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:36:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:36:55 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:36:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1030c456d04636112fa347ddc5296036cddf70c8085be2e3f3fb481898f18fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d0211bbd9a4fd28f739a797600d78394b15d947a30f55f70cfd5daf0f9e443`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1057c9a28776b9ab60a6a0a79afb37a5d68f1ec650c9c1a1e95a5e161d023c6`  
		Last Modified: Thu, 30 Jan 2020 03:43:35 GMT  
		Size: 11.8 MB (11833542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc0c32069403f3e0a4f55c207150573a3bb394b724b76dafdd8047fc23b5df3`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ae0e20a91aabdf806c18dbdd7d9fa57ff9451d8354fe67ceee55d856261711`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52891a1e287134685d008b61d9c2d00b7221a3e7bf5a538ee8d598dbab98415b`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade8b42d5008d85cee916e695a1da705b04a744722172eaabe685ec30c71382`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedc566e2fda6435ca2aaff8334c3690c8463e77cabfe275cc70ff7046f65686`  
		Last Modified: Thu, 30 Jan 2020 03:43:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:661bd96681eb4625bc7fba9559b8920adfb41f14e3ee51075f2b3190f6f136c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14040955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a667f9e70361ee42baff053b3ce63b6a84f42d24ba2055dc63ce2be52afc4047`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:49:35 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:49:36 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:49:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:02:30 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 03:02:31 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 03:02:33 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:05:14 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:05:17 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:05:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:05:20 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:05:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:05:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:05:23 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:05:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:05:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:05:30 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:05:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab27e2422be886bc0a338b0e0c20b8e2beea15b880defbac81f75c04495d0c2`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae2520a8d4cdac962b6d4a62335dce896f8ccb0b6d2693b0e72591fda026d14`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6dda155ab6da3f7ce5a0a095b31f550ad1eec7400f992ce356739d2cc13322a`  
		Last Modified: Thu, 30 Jan 2020 03:13:11 GMT  
		Size: 11.4 MB (11410503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fdb21a7a829d858ac12aa032091ca59612507b5c90725646c5d65e2cc94e7b`  
		Last Modified: Thu, 30 Jan 2020 03:13:02 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f35936da04d6e44ec4b999a8e2fd12bcd4005d87a9eb96247c6ba7e901b7593`  
		Last Modified: Thu, 30 Jan 2020 03:13:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cbc4d887b3f8ca246d14d7e7e74ad0fd37bdee30947d7c4476f44eed62cb6c`  
		Last Modified: Thu, 30 Jan 2020 03:13:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a449e0683710f8a1fc54b307dc9d12f86cc429d2e5dc3e172aa97d091612d6fe`  
		Last Modified: Thu, 30 Jan 2020 03:13:03 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed69b99af5471a2076c49109a08a03a3cf60bd9e4f6a7cb33f8914b3face753a`  
		Last Modified: Thu, 30 Jan 2020 03:13:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:539d79e1ab79b18f4aa35f9c3a393582b7a571fccbb817b66e9f6f243d679fc8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13210081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dee6416c8a156bc2a95d3dcbb4a01c07243238e50687f792a1b2f7260ca9c7c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:00:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:00:13 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:00:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:10:24 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 03:10:25 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 03:10:25 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:12:30 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:12:33 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:12:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:12:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:12:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:12:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:12:39 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:12:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:12:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:12:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:12:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572777a7d0992ea05b14f2ba3230ce906c753dd21eb73ac2b6018551250312db`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8810228251d658112d3dbf2b9b1719f402a0c3477bf2eceaa5a20341bba3f5`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4a4696e10febf1192fc41774e4996a9c99fab6cc6dd148f2c7e2baccb3d4c8`  
		Last Modified: Thu, 30 Jan 2020 03:20:02 GMT  
		Size: 10.8 MB (10777629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5dc0ebb7e5bcfad548b278494935b59ef68bb175ee5269bd651ac11b6165b9`  
		Last Modified: Thu, 30 Jan 2020 03:19:57 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fac1cf77ead444c3aae0b40bad245e46b67485edcb28fc5e68ca82ca5c20e`  
		Last Modified: Thu, 30 Jan 2020 03:19:56 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44def7b6fb7128bd73a57749b60c6494934f44a032a5853f4b33c8a7287272e3`  
		Last Modified: Thu, 30 Jan 2020 03:19:57 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11acc24b73cf50d5a7dfb16a359dcb3952f255a2c993b5cacfd45b093986e2d`  
		Last Modified: Thu, 30 Jan 2020 03:19:57 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a650ba71db65a089810172ab8b952fbffc483232cc4504228baa2e9c08712`  
		Last Modified: Thu, 30 Jan 2020 03:19:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:07e2b0c89d90a2656c012fd06b9f167ce78b02e5631aae0f06123354d4d119eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14413467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b984aa4f7ce2832012a15d76412facf070ed72cd310854291891c125daa07986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:40:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:40:28 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:50:49 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 02:50:50 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 02:50:52 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 02:53:26 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:53:28 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:53:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:53:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:53:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:53:40 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:53:40 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:53:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:53:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:53:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db837ff5778a13ace9e439e3bff33c317ecca84803a142a4ee4e05d2af54def`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92b445ab1ef4ba9a6120e5cc359b70cb88b74a46dee803f2709cb873a7be79`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c972a35f031edcc5519cb2d82fd3e75925c0f166bcc51cf07b5d0f6d6520ba98`  
		Last Modified: Thu, 30 Jan 2020 03:01:02 GMT  
		Size: 11.7 MB (11677499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e156b311e59e67533aa89c29ebbbf0010a90dfe599a91e461be03237bea41a28`  
		Last Modified: Thu, 30 Jan 2020 03:00:57 GMT  
		Size: 7.2 KB (7155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d8d5c59fcd5ec94c54bf9f2d43324ae4af5c52449b00a6340aa550fa1130e`  
		Last Modified: Thu, 30 Jan 2020 03:00:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e176c5ad16776b3ed9c78a826c56b6805805ea6c7de3dc1a6d9399cb77fa290`  
		Last Modified: Thu, 30 Jan 2020 03:00:56 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77b47d2704d263cad4b8f1e90c58d1d16d6227924428a9bdd1bdbf3cfeeeadc`  
		Last Modified: Thu, 30 Jan 2020 03:00:57 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a42e1479a8b7c8101baaa134ee430b65e5b52f4983a7624f61ca9224d0cb7c`  
		Last Modified: Thu, 30 Jan 2020 03:00:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; 386

```console
$ docker pull postgres@sha256:212041f986e8c8756149494defae89b95c815bfb0c152df58b975706ba4acb90
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15275660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0080c1225896c0760aefebf89f0b0664bcd8c29cdae559322541cea73b49e60d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:38:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:38:44 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:38:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:56:13 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 02:56:13 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 02:56:13 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 02:59:42 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:59:43 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:59:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:59:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:59:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:59:45 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:59:45 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:59:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 02:59:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:59:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:59:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb8463eb063fd24e3d29bd4ca5b9ba1590717acda7415cb45da3e7560f0dd`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023c33adbfeb9b779f40edac1617b4514e1fb0b976b5b201dd0f7dc688f5e60`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49f93678df794c61a1d72144fb23535044c306682a96aa160c18349e111b0a`  
		Last Modified: Thu, 30 Jan 2020 03:08:11 GMT  
		Size: 12.5 MB (12456337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b2cc2c8a06f7a47991da929b764b8d671a4080d9b01564fa8f7cd5007fdd7e`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 7.2 KB (7155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c720332a64317c5d72a640d63a9ac0b5762b9af6db25c51a53983c941f0861`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492617946eec1c296943b7dcd1d7940fb689d1b19b22aae530eeacf948352ef8`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a106bf288ba4d1ce2a3dd80535b186dc29df23524b0dbdc496b9026bf552c0`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1436738e877347996a2bf14590058d8173fbbf89605b47946030c9ad24f934`  
		Last Modified: Thu, 30 Jan 2020 03:08:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:928d7215380bbe77f4962bd9fefcfafd1e93e943b1a8293bb7808acce94499f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.6 MB (15557345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd7d92f86da623a8f2596cd1856ff14fbfa66184df49c00e77f6a7d7c3ef2c0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:20:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:20:03 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:40:19 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 03:40:22 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 03:40:27 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:43:14 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:43:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:43:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:43:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:43:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:43:40 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:43:41 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:43:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:43:59 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:44:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8af198a4c612619984a3d16dc2a9fb3f15835dfbf5269a9eab9a345ed4f14`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852af7c4759ead6b82b170b6d34d124532026b41ec5d7dc4ec99bd6705f633a`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658b58d94cab97c61d02b3a48350135284a608d0320139f7a5eee377c6243940`  
		Last Modified: Thu, 30 Jan 2020 03:54:41 GMT  
		Size: 12.7 MB (12722332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e35da3fdb3ab1ade3aef76ad7731b086f053589265905231456f7a1a3567b6`  
		Last Modified: Thu, 30 Jan 2020 03:54:34 GMT  
		Size: 7.2 KB (7153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610b71464c957c7cf7b312c32eb52c09d253138140ccea9ffa89349241933432`  
		Last Modified: Thu, 30 Jan 2020 03:54:35 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5add389f209669a388abb071108374100f053ce522b5774e1a1a0ecee1070f`  
		Last Modified: Thu, 30 Jan 2020 03:54:34 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d755d4533dbc318ffbb92b60488a2d0b77189f2f1040464217be65a9e40716c`  
		Last Modified: Thu, 30 Jan 2020 03:54:34 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4724b9087057f88efec97eb8bfd895b60bb8be28e19551d148bc87a0c96083`  
		Last Modified: Thu, 30 Jan 2020 03:54:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:7ec9d24814d44d459ec11cd58447428622859319979c3af4476e7346d385d7ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14249101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93326dfe2430e3ba3d2bd4878844bbc7b291b017f7c097e625bcf6e3c50fe2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:48:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:48:56 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:48:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:59:45 GMT
ENV PG_MAJOR=9.6
# Thu, 30 Jan 2020 02:59:45 GMT
ENV PG_VERSION=9.6.16
# Thu, 30 Jan 2020 02:59:45 GMT
ENV PG_SHA256=5c6cba9cc0df70ba2b128c4a87d0babfce7c0e2b888f70a9c8485745f66b22e7
# Thu, 30 Jan 2020 03:02:34 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:02:35 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:02:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:02:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:02:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:02:37 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:02:37 GMT
COPY file:abc85c5ac9d748ac5df3a643ab618de050dd65e8ef159dbdcdfe1a720ab1142b in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:02:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 30 Jan 2020 03:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:02:38 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:02:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d0ab56996305262d42136eee090848bbdf7cec28b8625e39078668b245db48`  
		Last Modified: Thu, 30 Jan 2020 03:07:31 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd3ab8f7e8df3f56e9628a504d2ea6db996a9910565bf84e3bc35bd847bcfb`  
		Last Modified: Thu, 30 Jan 2020 03:07:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a126ed3287b34fe720c506263021e7e31a184968e7ff47b009d604aa72ad689`  
		Last Modified: Thu, 30 Jan 2020 03:08:23 GMT  
		Size: 11.7 MB (11654177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188c64d812928562f857ddf834ec04f744e6003fab53071d9467debe4c5b5c4`  
		Last Modified: Thu, 30 Jan 2020 03:08:19 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45928fc7ce5df2ca490cd83d3b0913dd5c32a6f2b1a2d455c30b094bca7b555a`  
		Last Modified: Thu, 30 Jan 2020 03:08:24 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538d02a45edb1fc3ec2260fe2fab21efb3b212ea7ee5f94977c5876a845368d0`  
		Last Modified: Thu, 30 Jan 2020 03:08:19 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4df51723193fea68bd8c8f608c1a8fafa9818e3006e1eb2d8e8993485db490b`  
		Last Modified: Thu, 30 Jan 2020 03:08:24 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724156134ac6ffb3e96504c647e1f00d5d6d02bbf8f812d98a683f4c28c8ebf2`  
		Last Modified: Thu, 30 Jan 2020 03:08:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:alpine`

```console
$ docker pull postgres@sha256:686fc517b2b979f972aa2cdbdb4e3392f28b7d6e6dc31054c05144863e6d9098
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:alpine` - linux; amd64

```console
$ docker pull postgres@sha256:6d1510dc1fb520e346b9e653c77941ab3ad8db1081b519296dcfabfcf864d393
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60209239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76780864f8deb0b48cdde6aab3069e0735f5c19724a287d91ae7f448831a54e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:19:59 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:19:59 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:20:00 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 03:20:00 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 03:20:00 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 03:25:23 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:25:24 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:25:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:25:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:25:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:25:25 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:25:26 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:25:26 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:25:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1030c456d04636112fa347ddc5296036cddf70c8085be2e3f3fb481898f18fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:56 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d0211bbd9a4fd28f739a797600d78394b15d947a30f55f70cfd5daf0f9e443`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8060dfd57b68c41186b9460b303cc45b5e4d68bc8a0068700dec4f1bb0f47b`  
		Last Modified: Thu, 30 Jan 2020 03:43:04 GMT  
		Size: 57.4 MB (57392577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0905212eea51fe66acc2cd9fef63f91d73ffe7dfa3b27311ec4ec393b8fad2fe`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 8.2 KB (8211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a126b91cf92ff8940d9f65535c747079fee16d71c27618142eca0bac7ebebf5`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45f87d751e97454b063f18ded1bc280660fc1c616affdc0dc2210e9e805d446`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2148a93fc26ec6eb896ae6b4e0470106722e10feef81cbb83e6e8fe3459b4ec9`  
		Last Modified: Thu, 30 Jan 2020 03:42:55 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:e4109cdc27e39a043b52c2eeaa5ebccaec6c8dbe9929ec0e5b493cb6b391f459
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58622281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea62dec9853c1679984035cb61af6d5e93611140410ffb1967f8730b35850cd3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:49:35 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:49:36 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:49:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:49:38 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 02:49:38 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 02:49:39 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 02:54:02 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:54:05 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:54:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:54:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:54:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:54:11 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:54:11 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:54:13 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:54:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab27e2422be886bc0a338b0e0c20b8e2beea15b880defbac81f75c04495d0c2`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae2520a8d4cdac962b6d4a62335dce896f8ccb0b6d2693b0e72591fda026d14`  
		Last Modified: Thu, 30 Jan 2020 03:11:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a722cf47a5d9e2ecdbca0527baed31e0c969df84292cf7b4d535fb1ed008c1b`  
		Last Modified: Thu, 30 Jan 2020 03:12:06 GMT  
		Size: 56.0 MB (55990889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fabaa46778b33fd058aa9ad21f3a88457aa6a4bc2a7711c946041fdc5683b6`  
		Last Modified: Thu, 30 Jan 2020 03:11:48 GMT  
		Size: 8.2 KB (8212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2e893a8b4b319a0df20d5548433fdd1a8aa768ab6c43243613958c68b83a1`  
		Last Modified: Thu, 30 Jan 2020 03:11:48 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045aee12c861e00b0238d8fa98b0d9858380be6b06f99fa6b73132c5f8ccc384`  
		Last Modified: Thu, 30 Jan 2020 03:11:48 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25638010d03799556d44805f65a28ec0b551ba92c81e3ef6b0d758690bc1a44e`  
		Last Modified: Thu, 30 Jan 2020 03:11:48 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:490812945c2aafee90a8f4f030c79c1ac126eb3f2fdf1a49d9f36d77b0fae8ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55877719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff0f3c5a5f64747e220a0e46108b50a759ed99c694655c0779c8737815fbfa0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:00:10 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:00:13 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:00:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:00:15 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 03:00:16 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 03:00:16 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 03:03:18 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:03:27 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:03:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:03:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:03:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:03:43 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:03:44 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:03:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:03:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572777a7d0992ea05b14f2ba3230ce906c753dd21eb73ac2b6018551250312db`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8810228251d658112d3dbf2b9b1719f402a0c3477bf2eceaa5a20341bba3f5`  
		Last Modified: Thu, 30 Jan 2020 03:18:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0440024149898999f2925fad16d0906a5acaf582f137c092e6ffe492fba0050c`  
		Last Modified: Thu, 30 Jan 2020 03:18:53 GMT  
		Size: 53.4 MB (53444337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0b69a13b1e0d55e13b022cff4762658c1c132e7e09b8ee2c7abcd37a64731f`  
		Last Modified: Thu, 30 Jan 2020 03:18:33 GMT  
		Size: 8.2 KB (8213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d27ef35e1dd04911e24e1661facbedf0553fc74a1a30164404054b21070af51`  
		Last Modified: Thu, 30 Jan 2020 03:18:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4fb7b2447189f17d739416e48d823db0c6265efbd462c3b08af30f0127fec`  
		Last Modified: Thu, 30 Jan 2020 03:18:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8487f1ad10109177a9830bea21caf784094c75a928a54f20ffda4aa42081f7d`  
		Last Modified: Thu, 30 Jan 2020 03:18:33 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:50229cfdcf2f0e58017cbfee317b7d9f77dcba8adef0fc77d8cf075c146f72ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.8 MB (59816718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79852caddd0e2d71f36f8f8f7d04fcc9dfb82942f42a2f960e8cb8cff2b9fe4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:40:27 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:40:28 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:40:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:40:30 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 02:40:30 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 02:40:31 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 02:43:37 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:43:40 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:43:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:43:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:43:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:43:44 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:43:45 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:43:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:43:46 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:43:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db837ff5778a13ace9e439e3bff33c317ecca84803a142a4ee4e05d2af54def`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92b445ab1ef4ba9a6120e5cc359b70cb88b74a46dee803f2709cb873a7be79`  
		Last Modified: Thu, 30 Jan 2020 02:59:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc686d41f5bda50e8af88ab466c917d3719483d6e6cce75d4320d1f8e3a31ad`  
		Last Modified: Thu, 30 Jan 2020 03:00:04 GMT  
		Size: 57.1 MB (57079817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040995314274c90b4219ea0616a0fe8f55de7a69c460aa81f9d1e0842855591f`  
		Last Modified: Thu, 30 Jan 2020 02:59:47 GMT  
		Size: 8.2 KB (8211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2cb564210a010901427bc0ecc92a3c74aebe110023a4ac458573f844d68e11`  
		Last Modified: Thu, 30 Jan 2020 02:59:47 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a7e8cd95fdb8cb6e9e8e2eb11de181f434cba8ea5ed233f734c718ba17778f`  
		Last Modified: Thu, 30 Jan 2020 02:59:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c6872e0ae787aafd709d552a37c873e9aceeef6f134b7ca83fe97b33bea5c7`  
		Last Modified: Thu, 30 Jan 2020 02:59:47 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; 386

```console
$ docker pull postgres@sha256:2707fdc5fc7de80d491a50742a9c4d452880a6baccee46626165aa93ee2504c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63503075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a283ed7bc47149212e65b1e1b48ced1b0cd43db32bb395784d54916e84c43c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:38:44 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:38:44 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:38:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:38:45 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 02:38:45 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 02:38:45 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 02:45:21 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:45:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:45:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:45:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:45:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:45:24 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:45:24 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:45:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:45:25 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:45:25 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2cb8463eb063fd24e3d29bd4ca5b9ba1590717acda7415cb45da3e7560f0dd`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b023c33adbfeb9b779f40edac1617b4514e1fb0b976b5b201dd0f7dc688f5e60`  
		Last Modified: Thu, 30 Jan 2020 03:07:21 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12d7f06890c46cd61cdaa35d77c6620b9f7bd0e18f56ab12c7223573682c6e4`  
		Last Modified: Thu, 30 Jan 2020 03:07:33 GMT  
		Size: 60.7 MB (60682813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717eab95de5727f2647df81a3e623422d0d6da0f1a239f81f49beb29da19ed08`  
		Last Modified: Thu, 30 Jan 2020 03:07:20 GMT  
		Size: 8.2 KB (8212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8645372b3f8e19172b59c419fa904284db7569a7244dce048f107313a738098`  
		Last Modified: Thu, 30 Jan 2020 03:07:20 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74908cfa3379c7f9699b55c2f166404ea9145f670dfeb1ae9907f4eb422faa88`  
		Last Modified: Thu, 30 Jan 2020 03:07:20 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a2aa22249caa908445eff022e57e64ec35416b9c0813ad87742b6905026bea`  
		Last Modified: Thu, 30 Jan 2020 03:07:20 GMT  
		Size: 3.8 KB (3839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:0509f725b358344ddf92d48bdb36beaae366f0cf392d9d320380889e40c36ef8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62508393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec010b745eb40c664b023633d12d09ba4adf7c8a449a0b62dad251eb59f21d6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 03:20:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 03:20:03 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 03:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 03:20:09 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 03:20:11 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 03:20:14 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 03:28:11 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 03:28:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 03:28:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 03:28:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 03:28:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 03:28:47 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 03:28:48 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 03:28:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 03:28:52 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 03:28:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8af198a4c612619984a3d16dc2a9fb3f15835dfbf5269a9eab9a345ed4f14`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7852af7c4759ead6b82b170b6d34d124532026b41ec5d7dc4ec99bd6705f633a`  
		Last Modified: Thu, 30 Jan 2020 03:53:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968c03fdd050acad3b1036cc889688f376662a89a0e9377d86e585d3bec6e560`  
		Last Modified: Thu, 30 Jan 2020 03:53:37 GMT  
		Size: 59.7 MB (59672450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8270fe06fad89a92a1fcf843edb82f944e375302ce0a8645a769254afc6d12e`  
		Last Modified: Thu, 30 Jan 2020 03:53:23 GMT  
		Size: 8.2 KB (8205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b07968249434b685ebe4e9e31641af2993e2561ee3dd9de65086e82b85a1a6e`  
		Last Modified: Thu, 30 Jan 2020 03:53:23 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85aadd28933545b5713d7bba52777b3aae9f2cf1d6b72c031c0ab5abf34be6c`  
		Last Modified: Thu, 30 Jan 2020 03:53:24 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b1103f24667299f066a0e1d773d9e65ef0a85987c1f834be8534a9d7937659`  
		Last Modified: Thu, 30 Jan 2020 03:53:23 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; s390x

```console
$ docker pull postgres@sha256:4d0a554cff31942375880976aadb1bc9258873c3981187d00485d90e02e5f9a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62394435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f13f23ba24a8992c41390967d4fc5914ff22783fa9dd87a36934f29f906afaa2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Jan 2020 02:48:55 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Jan 2020 02:48:56 GMT
ENV LANG=en_US.utf8
# Thu, 30 Jan 2020 02:48:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Jan 2020 02:48:56 GMT
ENV PG_MAJOR=12
# Thu, 30 Jan 2020 02:48:57 GMT
ENV PG_VERSION=12.1
# Thu, 30 Jan 2020 02:48:57 GMT
ENV PG_SHA256=a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
# Thu, 30 Jan 2020 02:52:48 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm9-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Thu, 30 Jan 2020 02:52:51 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 30 Jan 2020 02:52:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Jan 2020 02:52:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Jan 2020 02:52:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Jan 2020 02:52:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Jan 2020 02:52:53 GMT
COPY file:74700c51dbcbbad39fbd303750c2ac04ac10f59a73a55171e1fd0dbae6c2f311 in /usr/local/bin/ 
# Thu, 30 Jan 2020 02:52:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 02:52:53 GMT
EXPOSE 5432
# Thu, 30 Jan 2020 02:52:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d0ab56996305262d42136eee090848bbdf7cec28b8625e39078668b245db48`  
		Last Modified: Thu, 30 Jan 2020 03:07:31 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd3ab8f7e8df3f56e9628a504d2ea6db996a9910565bf84e3bc35bd847bcfb`  
		Last Modified: Thu, 30 Jan 2020 03:07:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86991534af0dcfa73489dd57b1a295bc670d98a42a40efdfbf572f8d95ea269`  
		Last Modified: Thu, 30 Jan 2020 03:07:35 GMT  
		Size: 59.8 MB (59798579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fee2b3b6229935dc8ac2f31f799d5edf0262cd79292f61e84f4ed7aa3a882a`  
		Last Modified: Thu, 30 Jan 2020 03:07:43 GMT  
		Size: 8.2 KB (8209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692fa998ff3b5325e278680c19ae2154bb46299aa4be960e3c9fa9eeb9543a7d`  
		Last Modified: Thu, 30 Jan 2020 03:07:43 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa365558bb0a4cc0bb7369a209c91a15d37b4dfa15dd986008e7ac11382ac2ea`  
		Last Modified: Thu, 30 Jan 2020 03:07:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851b6155a6baaee4d9751e478b81242eb8d4b081df17ab10044012445ff8daa7`  
		Last Modified: Thu, 30 Jan 2020 03:07:43 GMT  
		Size: 3.8 KB (3837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:latest`

```console
$ docker pull postgres@sha256:5181eccc7c903e4f1beffa89a735cb7ed72e0c81d6c34c471552c3fa8bff0858
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:latest` - linux; amd64

```console
$ docker pull postgres@sha256:0d4312223e13e5282f99d413950aa35cd624999a8650ad088095fe50e412e0b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132459661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf879a45faaacd2806705321f157c4c77682c7599589fed65d80f19bb61615a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:05:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 06:05:57 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 06:05:57 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 06:06:10 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 06:06:21 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 06:06:22 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 06:06:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:06:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 06:06:31 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 06:06:31 GMT
ENV PG_MAJOR=12
# Sun, 02 Feb 2020 06:06:32 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sun, 02 Feb 2020 06:07:06 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 06:07:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 06:07:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 06:07:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sun, 02 Feb 2020 06:07:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 06:07:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 06:07:09 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 06:07:09 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 06:07:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 06:07:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 06:07:10 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 06:07:11 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b355dbb6c6ba49b1944319de07e58ca26244ec451633b9d7656e77d0df4b8b`  
		Last Modified: Sun, 02 Feb 2020 06:12:26 GMT  
		Size: 4.2 MB (4177987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d237363a1a91586c6e1ad9d62722a3d56ca984ba9f2873e138e8085acb6ea140`  
		Last Modified: Sun, 02 Feb 2020 06:12:24 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b9d2fde66f1f78cc87ed21cdb8b3baa700c780dc2fe92fcc012cb8a4e1f66`  
		Last Modified: Sun, 02 Feb 2020 06:12:24 GMT  
		Size: 1.4 MB (1358574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646492d166e7a9b48cc30447d45f13c7738076910bf6f30819aeeaa291810d33`  
		Last Modified: Sun, 02 Feb 2020 06:12:27 GMT  
		Size: 8.0 MB (7964389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50eeac6fd5fb8c3b933413c46ab8c37dd54763a866a5a4191a946b4f5e4f7f6d`  
		Last Modified: Sun, 02 Feb 2020 06:12:22 GMT  
		Size: 300.9 KB (300940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502963de6da85420287fa1c54411e4fa45a266d8cde698de5b962b3f02ab833d`  
		Last Modified: Sun, 02 Feb 2020 06:12:22 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7263f7627b9115c61347a0c10dd3ad98c8986878b1dba57276af6ce68d2a982`  
		Last Modified: Sun, 02 Feb 2020 06:12:22 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b135c7e429e5c80eb1930f02813862068f82563fea9acf9c0e9cbd86e2aba7`  
		Last Modified: Sun, 02 Feb 2020 06:12:49 GMT  
		Size: 91.5 MB (91547373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259a29a883ed61840fae1401f7af8f330a72e1b65c41d5f730df92429cdce564`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 8.9 KB (8945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b8f133c3f497f82fa1d3a8a59ed3f7d00f5aa9c7935a703d740b56710eb9a6`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e91678bd481c43532c7a173153bcecc0aea53dd55eef51e073a15b6808c88f`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15326bd3db004029e30f63c6193c06324af0d60d72e756195b3c62d2d3d65e23`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 3.8 KB (3834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aab6409ca4d25a8800cce887ab77be76cb19c699522dcbb430e9ba38b653746`  
		Last Modified: Sun, 02 Feb 2020 06:12:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v5

```console
$ docker pull postgres@sha256:e078eadc94b2b3179a43131b2ff17b09eb955d643c354aaf5a416d6a19f0890d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126421019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5426b72e8515ab0aaa576a6eeedf6eeb7b0267a5310a02106b3e8f5859597d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:34:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:35:01 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 18:35:02 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 18:35:23 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 18:35:44 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 18:35:46 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 18:35:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:35:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 18:36:01 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 18:36:02 GMT
ENV PG_MAJOR=12
# Sat, 01 Feb 2020 18:36:03 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sat, 01 Feb 2020 19:03:36 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 19:03:41 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 19:03:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 19:03:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 01 Feb 2020 19:03:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 19:03:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 19:03:46 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 19:03:47 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 19:03:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 19:03:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 19:03:50 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 19:03:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70006e2ae692e3a1d3eda514f0de630b9cd77673aeb976c1e8a02b73cf8b7264`  
		Last Modified: Sat, 01 Feb 2020 20:50:23 GMT  
		Size: 3.8 MB (3847808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51f7983f9190b3cf57e2162aaa536103797b7b2db41ec034ac1b7bb738a7db4`  
		Last Modified: Sat, 01 Feb 2020 20:50:22 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f43bd19defefde17a52fb094b49664f52f5d36d08e761452ab81b6daf3d2469`  
		Last Modified: Sat, 01 Feb 2020 20:50:22 GMT  
		Size: 1.3 MB (1318116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bee3c68ffa27d48c5e64724a11c9ce65500c467e37cd40b9d40bf6f7e7e08d`  
		Last Modified: Sat, 01 Feb 2020 20:50:24 GMT  
		Size: 8.0 MB (7965055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df868ae33379c795c154a8ddcc37740d3b7f827af475b18c68884116d795a66d`  
		Last Modified: Sat, 01 Feb 2020 20:50:20 GMT  
		Size: 298.7 KB (298736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6934c8d464038d8a2d408d443259cd545bbd9ffcb8ceab0dbb2342f96ab69711`  
		Last Modified: Sat, 01 Feb 2020 20:50:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520c13f9b7c083374a70fe0f3325f0bcb4088a5b3417e1c9bb794849aa00aa2e`  
		Last Modified: Sat, 01 Feb 2020 20:50:20 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90083940f769eb064647115deaab33448ab82d0c883c8a7e2e524135927d3e72`  
		Last Modified: Sat, 01 Feb 2020 20:50:49 GMT  
		Size: 88.1 MB (88143396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4f7f8266b1cda46a0d14eda5bc4bc6f097081c177b2cfc5037390692b136ba`  
		Last Modified: Sat, 01 Feb 2020 20:50:18 GMT  
		Size: 8.9 KB (8946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3c53c89257271a5f68c228e3cb27b34fca81d0c9ca4a5d434980c5bc52a8c1`  
		Last Modified: Sat, 01 Feb 2020 20:50:18 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b423b27e12af4ee04ae7a8fc7412ade0b6715816f633009fb0a3f1a361579631`  
		Last Modified: Sat, 01 Feb 2020 20:50:18 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00935b7e8f2d0afee05a0c6998f6111a1ae415e39e8c0c9ffe6dab1d0b726ba5`  
		Last Modified: Sat, 01 Feb 2020 20:50:19 GMT  
		Size: 3.8 KB (3833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2df8f298ce648d91a02e60522608117d44a826a68b45d09b962d07a279dc3f`  
		Last Modified: Sat, 01 Feb 2020 20:50:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v7

```console
$ docker pull postgres@sha256:7ccf4bc46e42d9279f0a20dd890c4b50d14a1fa42d0091346f7305ab09c8b0df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121935162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc1644763b76d135d79b7c008799fada6975721de94086a79e17d419baa2831a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:28 GMT
ADD file:8658fd39d2726b84ace6e940a73e3f5fdf03b339f01e8cca3166e44abe3f9ac3 in / 
# Sat, 01 Feb 2020 17:00:29 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 08:30:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 08:30:25 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 08:30:26 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 08:30:45 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 08:31:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 08:31:06 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 08:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 08:31:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 08:31:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 08:31:25 GMT
ENV PG_MAJOR=12
# Sun, 02 Feb 2020 08:31:26 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sun, 02 Feb 2020 08:57:06 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 08:57:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 08:57:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 08:57:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sun, 02 Feb 2020 08:57:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 08:57:21 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 08:57:22 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 08:57:23 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 08:57:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 08:57:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 08:57:26 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 08:57:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0c7074b2d47c15922db5c0eda14250224eb72756c800081d2b0627ffb369568d`  
		Last Modified: Sat, 01 Feb 2020 17:07:47 GMT  
		Size: 22.7 MB (22699138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d581d588bd5e2ca7c84216a9def839421358d391a572f06f6a6397329cd2e429`  
		Last Modified: Sun, 02 Feb 2020 10:35:59 GMT  
		Size: 3.5 MB (3481690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d38b43f6d701f50e329b3c3adb68cd87e49cd6bccf7be318997acc79745250a`  
		Last Modified: Sun, 02 Feb 2020 10:35:59 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1719f3ca6300f86e468242312c23adbde13edfb69da566acdb515d67e0285e58`  
		Last Modified: Sun, 02 Feb 2020 10:35:58 GMT  
		Size: 1.3 MB (1309493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12068913b9eadd4758fa283755c0081c35274d2d7b304257b3c8d3ecdc1dfcf3`  
		Last Modified: Sun, 02 Feb 2020 10:36:00 GMT  
		Size: 8.0 MB (7965114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a862a006e9d757167d50e3cdd87bff07997c60a8947751f7dce5764eb1c67b`  
		Last Modified: Sun, 02 Feb 2020 10:35:56 GMT  
		Size: 297.1 KB (297108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d204e55de65af43d3a5f2f4a58cb2967c012da696881f6598b097b8278d9f7`  
		Last Modified: Sun, 02 Feb 2020 10:35:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14994cf874f0aa45e27c3b9a97fdda202f094757880776a3295db75e4f8816a`  
		Last Modified: Sun, 02 Feb 2020 10:35:57 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1044ab3ecec33f97178aaf48e7315a37260d993e339fbe9918e68d0d1d9d793`  
		Last Modified: Sun, 02 Feb 2020 10:36:26 GMT  
		Size: 86.2 MB (86164394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6bb03ce7e1ff28a09268597b0d61d54f7a7f746e76e357b0819b0e6804fbd2`  
		Last Modified: Sun, 02 Feb 2020 10:35:54 GMT  
		Size: 8.9 KB (8939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dd490aee024ce23ca9ea1dab4fc770e1f20ffcaace82da79c98588ce10df6f`  
		Last Modified: Sun, 02 Feb 2020 10:35:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb67c8e5cb7606aa7f42b2e41ad8b1a6cf1194fd356447ea134d9c170f3c1e61`  
		Last Modified: Sun, 02 Feb 2020 10:35:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1182cce53f53d63a2af207b18aa6a8cd3471fa6791f310cdd5817d1849942e4`  
		Last Modified: Sun, 02 Feb 2020 10:35:54 GMT  
		Size: 3.8 KB (3832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb577abd486e9dbfc5d60bf46877ea34722caf1da72fc776927c2bfdc4c7444`  
		Last Modified: Sun, 02 Feb 2020 10:35:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:84e698fb4afa52b26cde4a2051a59c82588bea38db83482cc3f8a4f7ee80b618
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128797621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3303d3b3ff18b18cd346da028b5c910bfd08f33ed9853b6d4e174faa5134768d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:11 GMT
ADD file:cd38c10a494a1bdab0bab5baef1886651931e96b6db2d34ff4415660a299470f in / 
# Sat, 01 Feb 2020 16:41:12 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 01:55:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 01:55:56 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 02 Feb 2020 01:55:57 GMT
ENV GOSU_VERSION=1.11
# Sun, 02 Feb 2020 01:56:19 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sun, 02 Feb 2020 01:56:34 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 02 Feb 2020 01:56:35 GMT
ENV LANG=en_US.utf8
# Sun, 02 Feb 2020 01:56:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 01:56:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 02 Feb 2020 01:57:00 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sun, 02 Feb 2020 01:57:01 GMT
ENV PG_MAJOR=12
# Sun, 02 Feb 2020 01:57:02 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sun, 02 Feb 2020 02:23:05 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sun, 02 Feb 2020 02:23:10 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 02 Feb 2020 02:23:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 02 Feb 2020 02:23:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sun, 02 Feb 2020 02:23:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 02 Feb 2020 02:23:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 02 Feb 2020 02:23:17 GMT
VOLUME [/var/lib/postgresql/data]
# Sun, 02 Feb 2020 02:23:19 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sun, 02 Feb 2020 02:23:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 02 Feb 2020 02:23:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 02 Feb 2020 02:23:27 GMT
EXPOSE 5432
# Sun, 02 Feb 2020 02:23:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f7ca645dfd2fe61e7661b7f3b3951c589ccbff71aa054611475de455650bd8a8`  
		Last Modified: Sat, 01 Feb 2020 16:46:28 GMT  
		Size: 25.9 MB (25850659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f388bb0aa851f4bf41a6d4990a5b02f92e8dec9fb0a4bfb1ad69670c0499b56`  
		Last Modified: Sun, 02 Feb 2020 04:06:47 GMT  
		Size: 4.2 MB (4170031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfd56988f6c52fdcd2d9364dd5f02671bd03dca661e9cd79cb84e440d47f49c`  
		Last Modified: Sun, 02 Feb 2020 04:06:47 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a40467cb81173237a90ca7fd832b2f640fcc61df67de14b116d11155f21e6a`  
		Last Modified: Sun, 02 Feb 2020 04:06:46 GMT  
		Size: 1.3 MB (1292567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127f0bf8802acf134c98076466679b64c6e65cbf3b3bf84e6f5c7b7620e4906b`  
		Last Modified: Sun, 02 Feb 2020 04:06:47 GMT  
		Size: 8.0 MB (7965115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12f0ff25dd163f3615a82239240a6147716e292cebfa708b9df83d46c92b718`  
		Last Modified: Sun, 02 Feb 2020 04:06:44 GMT  
		Size: 297.2 KB (297199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baffb02ad63e236b4b1a60fe916f3283fdbcacc3c2fbe380b53af2dccd712429`  
		Last Modified: Sun, 02 Feb 2020 04:06:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cc9d652d0a38de69666934953e5af2321eb0f6a84afe690b94eb036738fd28`  
		Last Modified: Sun, 02 Feb 2020 04:06:44 GMT  
		Size: 3.1 KB (3051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c0f8af1fb17cc42a7066ea764d4747916604e67800c9acc53483c4396a429e`  
		Last Modified: Sun, 02 Feb 2020 04:07:09 GMT  
		Size: 89.2 MB (89203814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bcf88097d6a9a863d486a53f101e3a8a8a8079960a6eea1277c71e9068d4ef`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 8.9 KB (8945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e40f39b0845fc6dcec06ee81dc497da1637af40f8ae2581d38f218575c4522`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e82f218dc48db49d1cf10b85b8315ebe6d7545238b2d461c6109df8f197bf3`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae8120259ba3b59c5a6cae2887712e0bf2edd6a38b3703a6698417d22251353`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 3.8 KB (3832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13a9fbbe5768e499a5f52e3fc7141ebd64f3cf00682fc621ae6eeef194dd7c3`  
		Last Modified: Sun, 02 Feb 2020 04:06:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; 386

```console
$ docker pull postgres@sha256:15d2b662bf217b36a736f1d02def3998ad6fa9ccf4437443248dac4c7c6cba75
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133605313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:646513813d7977878d6723e3ae2482e4272085c4a7e6562428133c14aa19cf05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:35 GMT
ADD file:be03c936f8d9737b4167f6563785971b009f05e4e508eb8249b365a9fae7b0e8 in / 
# Sat, 01 Feb 2020 16:39:35 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:19:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:19:38 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:19:38 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:19:49 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:19:58 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:19:58 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:20:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:20:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:20:06 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:20:06 GMT
ENV PG_MAJOR=12
# Sat, 01 Feb 2020 21:20:06 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sat, 01 Feb 2020 21:20:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:20:40 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:20:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:20:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 01 Feb 2020 21:20:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:20:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:20:42 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:20:43 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:20:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:20:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:20:44 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:20:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:57b164929d223abf41064de94f9f53ca37ec9f09843646c80344ff10c302051a`  
		Last Modified: Sat, 01 Feb 2020 16:44:32 GMT  
		Size: 27.7 MB (27747052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9997cc045ec61684d5eec173034939f749331c09514c0f8f613d25d901dc1024`  
		Last Modified: Sat, 01 Feb 2020 21:26:55 GMT  
		Size: 4.5 MB (4542204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66be524cdc140df03dbcccd1a976d544f2e4829fc9bfc3e7bdccc89599795d6`  
		Last Modified: Sat, 01 Feb 2020 21:26:53 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398bfc0869d06d06235249409f9b9f5e47c7ce448f9d463d9a2cd70f0880bfc`  
		Last Modified: Sat, 01 Feb 2020 21:26:53 GMT  
		Size: 1.3 MB (1324297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655574080d822c8be4e7c5cae573ea8f54a9253cb9c1832c1f6a410992cc1ac9`  
		Last Modified: Sat, 01 Feb 2020 21:26:56 GMT  
		Size: 8.0 MB (7964334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855eb32a60e3afa4f766aa8d5c7bcf756848c25bad82dacab8e4c1b194a62c64`  
		Last Modified: Sat, 01 Feb 2020 21:26:52 GMT  
		Size: 302.6 KB (302646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a231a2303f474ca777cfd033c48642e0697ef96ae78a91b7b1c8c06efa2adf`  
		Last Modified: Sat, 01 Feb 2020 21:26:52 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4d191a2ed807914eb97dedc8af739d87405c38a5cfe6253ef03b94e55f8466`  
		Last Modified: Sat, 01 Feb 2020 21:26:52 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540bef7e7e0ebb599b2a52cbbcf6bba8d0abb411477c3e8929b6a8893259d049`  
		Last Modified: Sat, 01 Feb 2020 21:27:23 GMT  
		Size: 91.7 MB (91706653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416302b0bdc10382b71f0422598b309abcb0431d26a98bf11af535d507ddf148`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 8.9 KB (8939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01dd73843a8b777c3d04e4d985aeed22fb46c77680776bd824fe84ca758284a`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26acb787c93edcdaad18e008fb60074aea01398dd3c30de4a95edf9f0c92e76`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278773a18c87177bdf3a45a07849805beba861ad6b22d2955f3ce51c6d4c40de`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6d274516a60cf901e0dd529b59c13ed19cc956416fb0083500adee1cae5d5e`  
		Last Modified: Sat, 01 Feb 2020 21:26:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; ppc64le

```console
$ docker pull postgres@sha256:215dc5d6669a1da21d5b3085c2c7c9f38535f79d1623bcaa1abfc4b11037703f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.7 MB (140661747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ea846050bcc433b0a867bdae9ea6aff85550d9cb39c9fd19babe6daa05d55d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 17:18:04 GMT
ADD file:aadd94011800934ec665edb193029ab2be0aeb668c566ba4bc52bd678e71a735 in / 
# Sat, 01 Feb 2020 17:18:06 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:28:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 22:28:51 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 22:28:55 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 22:29:39 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 22:30:02 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 22:30:05 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 22:30:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:30:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 22:30:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 22:30:39 GMT
ENV PG_MAJOR=12
# Sat, 01 Feb 2020 22:30:42 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sat, 01 Feb 2020 22:33:08 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 22:33:19 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 22:33:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 22:33:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 01 Feb 2020 22:33:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 22:33:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 22:33:38 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 22:33:39 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 22:33:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 22:33:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 22:33:49 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 22:33:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:16a7e1c5b23ec3cf93421f5f868c1cf2cda468cfebb1b2bc62f4d533d99d256b`  
		Last Modified: Sat, 01 Feb 2020 17:26:05 GMT  
		Size: 30.5 MB (30517693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4887b42e3fa4bab4b6a923a23616405501ac3a66a9980379276a018032fcba51`  
		Last Modified: Sat, 01 Feb 2020 22:57:21 GMT  
		Size: 5.0 MB (4967152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27430705fd8e84fe0517512f555ef1ba8cc7a678cb11ec355b1cb20c6fc5a86a`  
		Last Modified: Sat, 01 Feb 2020 22:57:17 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dfdcc823e3bdc8b3c097c0692c8d7e18bac53a5c81d492ab4a0459851d8f1d`  
		Last Modified: Sat, 01 Feb 2020 22:57:16 GMT  
		Size: 1.3 MB (1281132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec861509b6b231e57138dbd3e70c457a6e9a37723dab364034f3db3132efdeb`  
		Last Modified: Sat, 01 Feb 2020 22:57:17 GMT  
		Size: 8.0 MB (7965285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8d1e2714f7c11d0d4f86e45f6b4c185ab5415036ce792cc5458b1f7d2d040f`  
		Last Modified: Sat, 01 Feb 2020 22:57:13 GMT  
		Size: 298.4 KB (298419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace9017f0ac376a5945ff5e4539ed18191f8a3ed9393442110a476621cc0e02a`  
		Last Modified: Sat, 01 Feb 2020 22:57:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4835b320e4b6d061c58f94a862d753376ee1cb29e6121a43896fd5a14aafb8`  
		Last Modified: Sat, 01 Feb 2020 22:57:11 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745126f068ad315829ea29cbf2653902b92bee847d70eb57f54bc98f8f8fbc11`  
		Last Modified: Sat, 01 Feb 2020 22:57:35 GMT  
		Size: 95.6 MB (95613824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64bea14266964a29c5e52db3dc270408dc11e05737b1984557ebd3a681d662e`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 8.9 KB (8946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67701b86081c69f032a3e349694d7fae90ab23601989775860189405fc7e0f4`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0f69553453dbae98a758499e7f56e80bcb8c2f5974e75e19bc0dedeb4173c0`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e22e6b585a6acc8c623bcc1df9162d64414d3e450c536420781a505eb317e51`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 3.8 KB (3836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d1338c638f8b6969a45c4e701eae1e7fe15b618b7b2d6b3f81923114c1d439`  
		Last Modified: Sat, 01 Feb 2020 22:57:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; s390x

```console
$ docker pull postgres@sha256:fd2eeeccb8821e23ef204c28a973d77bb9f8df17f2ffecf013902e072cd242a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130699858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4c8412c11232f198d75c5bda5db095c94996b1e967df11d477642f88e37d09f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 21:31:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 21:31:16 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 01 Feb 2020 21:31:16 GMT
ENV GOSU_VERSION=1.11
# Sat, 01 Feb 2020 21:31:27 GMT
RUN set -x 	&& apt-get update && apt-get install -y --no-install-recommends ca-certificates wget && rm -rf /var/lib/apt/lists/* 	&& wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture)" 	&& wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$(dpkg --print-architecture).asc" 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 	&& gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu 	&& { command -v gpgconf > /dev/null && gpgconf --kill all || :; } 	&& rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc 	&& chmod +x /usr/local/bin/gosu 	&& gosu nobody true 	&& apt-get purge -y --auto-remove ca-certificates wget
# Sat, 01 Feb 2020 21:31:32 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 01 Feb 2020 21:31:33 GMT
ENV LANG=en_US.utf8
# Sat, 01 Feb 2020 21:31:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends libnss-wrapper; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 21:31:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 01 Feb 2020 21:31:38 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 01 Feb 2020 21:31:38 GMT
ENV PG_MAJOR=12
# Sat, 01 Feb 2020 21:31:38 GMT
ENV PG_VERSION=12.1-1.pgdg100+1
# Sat, 01 Feb 2020 21:39:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64|i386|ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Sat, 01 Feb 2020 21:39:44 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 01 Feb 2020 21:39:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 01 Feb 2020 21:39:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 01 Feb 2020 21:39:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 01 Feb 2020 21:39:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 01 Feb 2020 21:39:45 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 01 Feb 2020 21:39:46 GMT
COPY file:4d8b208323038919c8c9e9cfc2054aa4608310078b03dae8cb6c8af58d89b616 in /usr/local/bin/ 
# Sat, 01 Feb 2020 21:39:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 01 Feb 2020 21:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 01 Feb 2020 21:39:47 GMT
EXPOSE 5432
# Sat, 01 Feb 2020 21:39:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74fefbeeb6df5424be490954827987a8c7927e23533e2b454167f45022c7af5`  
		Last Modified: Sat, 01 Feb 2020 22:14:51 GMT  
		Size: 4.1 MB (4059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895f0676ff0f3afd82aec3a77b255c9c0c581b5e803f23827986d19fc5f6f50a`  
		Last Modified: Sat, 01 Feb 2020 22:14:49 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e654e4a94e69c38789dc3333f9302ae6da13fd5ad94357b844ac9ca012bc21e`  
		Last Modified: Sat, 01 Feb 2020 22:14:49 GMT  
		Size: 1.3 MB (1347168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85405aa2bd96afbcab08a204fb2728b768360ce8825d8a11b53b859cdc28076a`  
		Last Modified: Sat, 01 Feb 2020 22:14:50 GMT  
		Size: 8.0 MB (8019246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a965d11c59c3785fdb3ffab95e8098799bc345f0d290afccacaf7062100d5b`  
		Last Modified: Sat, 01 Feb 2020 22:14:47 GMT  
		Size: 299.5 KB (299520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa6431faedce67353c59a7a1f079a4562b05844dc6695c00abf4e0eb3d5b27e`  
		Last Modified: Sat, 01 Feb 2020 22:14:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eee97bd06c29e84244a7eab8914aa3778a4e89a8624ad8f965739a260dd35d4`  
		Last Modified: Sat, 01 Feb 2020 22:14:48 GMT  
		Size: 3.0 KB (3048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e608d8ade99e94ba7d5615dcdf94f6a2f1df41bdece8d052a8dc8e99704587`  
		Last Modified: Sat, 01 Feb 2020 22:15:01 GMT  
		Size: 91.3 MB (91250606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76288b6b5963a068ab28c11a4c31b8bcdb74553d6d61099a513ba7f8ec6d71c`  
		Last Modified: Sat, 01 Feb 2020 22:14:46 GMT  
		Size: 8.9 KB (8943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80abcd2ec4ac20a6cddc78ea6bc2b361b62ecc324287f3b01493fac33c890361`  
		Last Modified: Sat, 01 Feb 2020 22:14:46 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7973374d8873226e1a70e8b705ef61c6a1dfef5bdd5254c521ab4df02b372013`  
		Last Modified: Sat, 01 Feb 2020 22:14:46 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0bff87841570aa5384d2c2f7e95d968007d37842dd2d58798cc450ed1e997d`  
		Last Modified: Sat, 01 Feb 2020 22:15:01 GMT  
		Size: 3.8 KB (3835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649ee830e8ce7dd8e5796449373587307b40da2a6d372f7a6745d95aa7f83887`  
		Last Modified: Sat, 01 Feb 2020 22:14:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
