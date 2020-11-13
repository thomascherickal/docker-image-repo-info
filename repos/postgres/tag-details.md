<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `postgres`

-	[`postgres:10`](#postgres10)
-	[`postgres:10.15`](#postgres1015)
-	[`postgres:10.15-alpine`](#postgres1015-alpine)
-	[`postgres:10-alpine`](#postgres10-alpine)
-	[`postgres:11`](#postgres11)
-	[`postgres:11.10`](#postgres1110)
-	[`postgres:11.10-alpine`](#postgres1110-alpine)
-	[`postgres:11-alpine`](#postgres11-alpine)
-	[`postgres:12`](#postgres12)
-	[`postgres:12.5`](#postgres125)
-	[`postgres:12.5-alpine`](#postgres125-alpine)
-	[`postgres:12-alpine`](#postgres12-alpine)
-	[`postgres:13`](#postgres13)
-	[`postgres:13.1`](#postgres131)
-	[`postgres:13.1-alpine`](#postgres131-alpine)
-	[`postgres:13-alpine`](#postgres13-alpine)
-	[`postgres:9`](#postgres9)
-	[`postgres:9.5`](#postgres95)
-	[`postgres:9.5.24`](#postgres9524)
-	[`postgres:9.5.24-alpine`](#postgres9524-alpine)
-	[`postgres:9.5-alpine`](#postgres95-alpine)
-	[`postgres:9.6`](#postgres96)
-	[`postgres:9.6.20`](#postgres9620)
-	[`postgres:9.6.20-alpine`](#postgres9620-alpine)
-	[`postgres:9.6-alpine`](#postgres96-alpine)
-	[`postgres:9-alpine`](#postgres9-alpine)
-	[`postgres:alpine`](#postgresalpine)
-	[`postgres:latest`](#postgreslatest)

## `postgres:10`

```console
$ docker pull postgres@sha256:8f14682f49a66eb10dd97a3336224e6136b33179e9569cd7d1bd999f40355e55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:10` - linux; amd64

```console
$ docker pull postgres@sha256:36e029a0132d40e6b6ae7f28369a64e59f4c80b89c48715fcf6af3d7bf93e130
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73132719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfd168e7b612255fcee87fff1fa7229e2245e9810a20ccd3b206b44f3c39d03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:33:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:33:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:33:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:33:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:34:01 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:34:02 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:34:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:34:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:34:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:35:19 GMT
ENV PG_MAJOR=10
# Tue, 13 Oct 2020 12:35:19 GMT
ENV PG_VERSION=10.14-1.pgdg90+1
# Tue, 13 Oct 2020 12:35:43 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:35:44 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:35:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:35:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 13 Oct 2020 12:35:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:35:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:35:46 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:35:47 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:35:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:35:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:35:48 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:35:48 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:35:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0526c44df6ea5bd7668eab6d9c37d43aef6474cb4f5b6d2539e82404a3827041`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 4.5 MB (4502050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2466ee00e96ac149c287cdd533cecad2907d0aea2f2fe5ffc7a706ab313aaac`  
		Last Modified: Tue, 13 Oct 2020 12:38:27 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c605d60192c83f6a890b4f0cfaf8d80cf2a7a5c0c8df01451a106305748bf2`  
		Last Modified: Tue, 13 Oct 2020 12:38:28 GMT  
		Size: 1.4 MB (1412112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b14ab418421f0d1e9fb147720201f216050e2ad983640a446e75249e84e9bc`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 6.2 MB (6182797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f557fff31511f1f9475342998e8b195c0942480fb4901dab214f015d2224c`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 384.9 KB (384916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bba27806f46c2448fe4d5a0b248fd9178ced6163b8e2154e4b06a86c9a08b4`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e1555090548b1ab5739971b4eea16b502cc1e625f3a0b827463c4ae69bcc61`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8228dd9c6c0d1dcfe71c2bda79b37e53b782fa9398bd43b5c7dc40f30cdb18`  
		Last Modified: Tue, 13 Oct 2020 12:39:00 GMT  
		Size: 38.1 MB (38108806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687446f7ecc1c7894784cbd2f305cbd8820505e9400501d9dcba2953e921c813`  
		Last Modified: Tue, 13 Oct 2020 12:38:49 GMT  
		Size: 8.0 KB (8015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3cd5a196d798f87557379c98dacf1c18fc5547f99d337cbc968fc22ca25993`  
		Last Modified: Tue, 13 Oct 2020 12:38:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed343704369a9dbf562aa5b6c93dc4b4e8454648eaacda6311aa44c7306f226f`  
		Last Modified: Tue, 13 Oct 2020 12:38:49 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd793ab304ef384e6ceae1445d5ade596bc7223947182063051541f84663077d`  
		Last Modified: Tue, 13 Oct 2020 12:38:49 GMT  
		Size: 4.3 KB (4267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d7b347c7d509389d0ce574f09fee172ec0ef11ebf91f82342d09ce996559fd`  
		Last Modified: Tue, 13 Oct 2020 12:38:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; arm variant v5

```console
$ docker pull postgres@sha256:7ed04f0338a5bd28e0d191f9768c664ac55c51fbc2dca304f0cafb94d5ae6db9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70100146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a7420c9c6ae0cb30c1df90893c055bcb8e893836b9fdd7eab349045835c7ad1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:57:28 GMT
ADD file:ef761876435f34dd5e73f6fb89eda5cee26b26d9183a37dc5588c6eb5fd4ba69 in / 
# Tue, 13 Oct 2020 01:57:29 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 07:10:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 07:10:23 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 07:10:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 07:11:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 07:11:15 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 07:11:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:11:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 07:11:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 07:33:55 GMT
ENV PG_MAJOR=10
# Tue, 13 Oct 2020 07:33:55 GMT
ENV PG_VERSION=10.14-1.pgdg90+1
# Tue, 13 Oct 2020 07:54:43 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 07:54:48 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 07:54:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 07:54:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 13 Oct 2020 07:54:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 07:54:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 07:55:00 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 07:55:01 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:55:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 07:55:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:55:07 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 07:55:08 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 07:55:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e6fa5ab8c49c07aa49f655f00f7742fc2640bec642d3e0b440a9d67c37d1383e`  
		Last Modified: Tue, 13 Oct 2020 02:05:36 GMT  
		Size: 21.2 MB (21194476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4a7d58f9de066b4eb914552800ca9b9c3bdbd3a49d22592a568fd65353b60e`  
		Last Modified: Tue, 13 Oct 2020 08:37:11 GMT  
		Size: 4.2 MB (4238677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d9d67c7f2447a0677783317716fd66e891874c5dec4c300963bdaedef3db73`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8dfd96a4ee2041e6cf18fbfb05eaaf56b746f396297762c746643158da072a`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.4 MB (1371374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55137faf878bb43f0e314a0845bb679c3834709fb30668a8a966d3ea7d6324c6`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 6.2 MB (6185655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c626e10cc735d164b870d78d396556ebae2e833924a9782fc8880333228fea`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 385.1 KB (385110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5193a2411b31608c76d06bf9efa210a7cf0d1b51953e39d3cdc458342b259a86`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71923a948044364e5093b7b7e4e2667ee46f8e6fc34ff01d72050cd7aefbe702`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 5.3 KB (5350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75be737d97efc465c92ea992842013bfe4b91aa43e72174472bdfff810fe44d3`  
		Last Modified: Tue, 13 Oct 2020 08:37:42 GMT  
		Size: 36.7 MB (36704806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1981c40a64d77d90a9c790c393cc669aaef81d9ec9621c4c928ef89b61236f`  
		Last Modified: Tue, 13 Oct 2020 08:37:27 GMT  
		Size: 8.0 KB (8022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6caf31c816dc4532cabbc94368f213e9ab617492902524ccaf93643dbf7cc530`  
		Last Modified: Tue, 13 Oct 2020 08:37:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f24907f918dd888afe46d98b2d7f6e93c819ec8ef5cc49e5aaa9fca6f58a468`  
		Last Modified: Tue, 13 Oct 2020 08:37:27 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fb36e52d3f1b51d175d6cf1f4cdf0eeb5145125ac87dba79698f74f9c64286`  
		Last Modified: Tue, 13 Oct 2020 08:37:27 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e2e45ceef8645aa5985eb4a0c5e8b2cced630b9af55e0e5b64dcb1b4b9dabb`  
		Last Modified: Tue, 13 Oct 2020 08:37:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; arm variant v7

```console
$ docker pull postgres@sha256:cb281e8c922ff149d791c24f238294fc1f11f7bf17b3f2288bd210d7f6e3b88e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66768261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80b859be3716f02765f3e470d5daa3ed6f3d6d3aad146cd300c0a6a04ec68534`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:04:30 GMT
ADD file:d204a257433edcd6f9ddd2c769b9e187c408eb4972203a5daab60214b5b576bc in / 
# Tue, 13 Oct 2020 01:04:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:54:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:54:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:54:44 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:55:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:55:24 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:55:25 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:55:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:55:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:55:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 06:14:25 GMT
ENV PG_MAJOR=10
# Tue, 13 Oct 2020 06:14:26 GMT
ENV PG_VERSION=10.14-1.pgdg90+1
# Tue, 13 Oct 2020 06:32:17 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 06:32:20 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 06:32:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 06:32:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 13 Oct 2020 06:32:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 06:32:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 06:32:27 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 06:32:28 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:32:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 06:32:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:32:35 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 06:32:36 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 06:32:37 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cc11be355171b10881b3ed16be16ceb2d7787cd459c6489d83bac55ee5824b35`  
		Last Modified: Tue, 13 Oct 2020 01:12:46 GMT  
		Size: 19.3 MB (19304540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8b70af887483c86f21ffd35a2a331fbab0ae0804a4929517360da6207fe6c3`  
		Last Modified: Tue, 13 Oct 2020 07:09:01 GMT  
		Size: 3.9 MB (3874946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09233e1347145a65db2aae548df648e91df34bde91664ac04509ff8ba2d77447`  
		Last Modified: Tue, 13 Oct 2020 07:08:59 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a09c7350562aee4559820b5fa1133618b8c02e7848e0c14635fb483b5a10fb`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 1.4 MB (1363819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9deba20fbd610072e97a51ac7766bcfdac37c6110ee53cdf296e7435868b5e7`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 6.2 MB (6185495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a750e8984fdec76cc5aa76a7979cd403c03d5b18efe690ebda5984356654554`  
		Last Modified: Tue, 13 Oct 2020 07:08:58 GMT  
		Size: 379.2 KB (379196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bd92fced2d524fc75c7429ca11a3f1c30587399ca0a571b4f623a3db6c15c2`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059b3634dc4169b9d362c9bf8d29e4c9af7a58bd40538452efeb506841942fb4`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab24877765e96c2e2033107b92348adca95488b43b0c0267027841c3ea83ae8`  
		Last Modified: Tue, 13 Oct 2020 07:09:33 GMT  
		Size: 35.6 MB (35640216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8637a66edfdc0f4e5a912de129783540ab4d6d2f06a2a5e52aade076209214e`  
		Last Modified: Tue, 13 Oct 2020 07:09:19 GMT  
		Size: 8.0 KB (8023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da15b1fc34ca21e81d2debb586b6a6c9cbf8919d59c90128e8a18e0a6e0cdbd8`  
		Last Modified: Tue, 13 Oct 2020 07:09:19 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a45074e58e270e2cf764f137dcf881b5af728761e7eb1135d8c04933df795`  
		Last Modified: Tue, 13 Oct 2020 07:09:19 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1ea10ed7a4f6fc388dd206d88761373a6853ac605cbe94a23376e0cd478761`  
		Last Modified: Tue, 13 Oct 2020 07:09:19 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f8bb3a194ac3db25225abef8c3f62a0cbd120dd65f1eb62eb56920aa53ce15`  
		Last Modified: Tue, 13 Oct 2020 07:09:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:53960bc4f1e841a47707fb94eae60e71d5a5aa714bcca074fba6ec15a256aa42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69383345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5fc08c5c861b0393ffce70b27ce6693fc60d18f551108530fed9f9bab8b473`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:21 GMT
ADD file:1783101ec41dba711940487fb45a9287f74a0639658051ad8bc9b2618a15be61 in / 
# Tue, 13 Oct 2020 01:44:22 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:04:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 11:04:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 11:04:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 11:04:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 11:05:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 11:05:06 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 11:05:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:05:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 11:05:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 11:23:52 GMT
ENV PG_MAJOR=10
# Tue, 13 Oct 2020 11:23:53 GMT
ENV PG_VERSION=10.14-1.pgdg90+1
# Tue, 13 Oct 2020 11:42:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 11:42:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 11:42:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 11:42:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 13 Oct 2020 11:42:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 11:42:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 11:42:21 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 11:42:21 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 11:42:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 11:42:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 11:42:25 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 11:42:26 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 11:42:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f4bec48cdb322f1180477bdd362bcd92d70a1ab628fc36319017bf4e8058d9ee`  
		Last Modified: Tue, 13 Oct 2020 01:51:12 GMT  
		Size: 20.4 MB (20376997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984be4b3fed9808b066a7600d2e83efbfd0ff4bfc1069a9d0814be2fd022f357`  
		Last Modified: Tue, 13 Oct 2020 12:20:59 GMT  
		Size: 4.1 MB (4078528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859bbaaf4e29eade0fbd81b43a64e5eb25198a55ef466f821ac3ba984a0bab4`  
		Last Modified: Tue, 13 Oct 2020 12:20:57 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882cfdcc3440ef89e60ecc554c9e53baa9bbbc241e2b37005dcd3d8f1faabdc9`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 1.3 MB (1346994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a8ef2ba5300bad73627e9166d141b0a67a7ad8d42cb3453893fb5f5813dea`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 6.2 MB (6185301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652a08bb6feda1aad8370161437fc26c9908787e595304676ceb34feafbbe901`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 377.9 KB (377937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17111fdbd30125a36e0c8429df7d3ff1c54dfe90c2c0999e2f3738dc89019f00`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed1a1a2b06a19d02a8d4d5890f949a8a250c418de647be680f045f2240fd2e3`  
		Last Modified: Tue, 13 Oct 2020 12:20:51 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc2fe6beccc80d7baaac3a2e642827478446e7e0a54b1e7985237b8c2ae0835`  
		Last Modified: Tue, 13 Oct 2020 12:21:24 GMT  
		Size: 37.0 MB (36997541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef9368dc69f26dc9021f3608381919159030ee0a3f4841b964b36e015fea732`  
		Last Modified: Tue, 13 Oct 2020 12:21:11 GMT  
		Size: 8.0 KB (8021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59c41edb6c5e1be4f7a95f3047f7bddac1208850a702edd1d1f7237836facf9`  
		Last Modified: Tue, 13 Oct 2020 12:21:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159a38457b112378f5d8852037493c62177d11f34c92963ad9f004c96a29befa`  
		Last Modified: Tue, 13 Oct 2020 12:21:11 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae01ac6623be8eca682efdeed84b2c3366612e3c5b620aa08f3abbc0b4f2f2b`  
		Last Modified: Tue, 13 Oct 2020 12:21:11 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece0e3435d1a539488df17041b6ed00481974fc8d804555d1c2ba76e760fd140`  
		Last Modified: Tue, 13 Oct 2020 12:21:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10` - linux; 386

```console
$ docker pull postgres@sha256:f49cc208bfa95a97261c7130a66390da6fbe506ac83249d7a4587af6be9ae034
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74311161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f6f9e3641510cd3b306eb77a44037696bcf68e0409af0a56ba7d4c45cbe264`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:45:31 GMT
ADD file:f09276bb607e6d68dcb997c1e8b4d004b91548964306d6a803286ba851484579 in / 
# Tue, 13 Oct 2020 01:45:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 16:43:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 16:43:18 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 16:43:18 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 16:43:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 16:43:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 16:43:49 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 16:43:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:43:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 16:44:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 16:44:55 GMT
ENV PG_MAJOR=10
# Tue, 13 Oct 2020 16:44:55 GMT
ENV PG_VERSION=10.14-1.pgdg90+1
# Tue, 13 Oct 2020 16:45:15 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 16:45:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 16:45:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 16:45:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 13 Oct 2020 16:45:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 16:45:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 16:45:19 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 16:45:19 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 16:45:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 16:45:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 16:45:21 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 16:45:21 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 16:45:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:02448e4a5fa68035acff67a00ba04305cbad42b25ffeb4b141c5f1f0b9d63a2a`  
		Last Modified: Tue, 13 Oct 2020 01:52:11 GMT  
		Size: 23.1 MB (23148149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1707623e5e9b92a3f43f1910a43ad9872060b853d07ecbf2b9b5bc02300501`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 4.8 MB (4809899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7908ca805e2bd89c5f1fe55e4f313469b7d84f6d049e59bc673439f8323b1d`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebde576b2c220dc444db8fcec0278f11a1df5bce6d091728aa378f74bb22734e`  
		Last Modified: Tue, 13 Oct 2020 16:48:40 GMT  
		Size: 1.4 MB (1382391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f9c2ca0b45e9e11f84e7f98ba02d277d65687fd873580517a5f0e50e6d7aac`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 6.2 MB (6182990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd5fdfe0405da8b45de435a650073673e910b7bd9545f2a05811eed28824401`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 393.2 KB (393233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3263197a4dd54e9fefd6e411e83b19f4186837e5aa15ce30c389245a5f7ae727`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1249d81ef1b333d5c1caf34a641e9466c3351724f2e669c983df59e95e4571`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde3cc5e04a6374f6448d88956e27e3fb33adda826fde7b525a5f4209956703f`  
		Last Modified: Tue, 13 Oct 2020 16:49:32 GMT  
		Size: 38.4 MB (38374562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0903dbd54ab05129fa1b9459a824c859a4204e907bdbb943aba536aa045d3abd`  
		Last Modified: Tue, 13 Oct 2020 16:49:17 GMT  
		Size: 8.0 KB (8017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790006b19df2d486822bdd109994bf4a3c18bffa6a48b97cfc7fb1aa746f7684`  
		Last Modified: Tue, 13 Oct 2020 16:49:17 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c69596bc4178c5b4d73f4e1a3c785f6dca3827a3633435b842fc9a05146483`  
		Last Modified: Tue, 13 Oct 2020 16:49:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dcf8181769c69bf9b8c025d8b04016d05e7548aa27c956821879daac0222c6`  
		Last Modified: Tue, 13 Oct 2020 16:49:17 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767db4741efb9b79afc8a777ea2a546314823f115dea0b088c648a0e1dc29295`  
		Last Modified: Tue, 13 Oct 2020 16:49:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:10.15`

**does not exist** (yet?)

## `postgres:10.15-alpine`

**does not exist** (yet?)

## `postgres:10-alpine`

```console
$ docker pull postgres@sha256:ce711e7269bcb351f8bf7109d7eee4211c7b540c4dc863802b8ba28f6dc41391
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
$ docker pull postgres@sha256:2f9531f73f9b7e44add79a827b46f0124471bbce28e79e126296ae4d9edf1c79
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28382400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72516014d1a3be53fbc6d1762b672049ebd9990e16955ce0179aafe851b8c241`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:55:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 07:55:14 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 07:55:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:12:22 GMT
ENV PG_MAJOR=10
# Thu, 22 Oct 2020 08:12:23 GMT
ENV PG_VERSION=10.14
# Thu, 22 Oct 2020 08:12:23 GMT
ENV PG_SHA256=381cd8f491d8f77db2f4326974542a50095b5fa7709f24d7c5b760be2518b23b
# Thu, 22 Oct 2020 08:15:22 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:15:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:15:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:15:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:15:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:15:24 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:15:25 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:15:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:15:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:15:26 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:15:26 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:15:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f1d1b70e7fa650fd6229086120f763219adce9e33e8b20bdfbf8452ab69847`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4f01476d2b86761cdb0414c4a583b89af3b5d0b67022cfc0d378743307f7e3`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd041b20444e5edf445dc83873fe065fa9a035fd8c39b89ccc17f82e1e459a6c`  
		Last Modified: Thu, 22 Oct 2020 08:22:55 GMT  
		Size: 25.6 MB (25572143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754d1cc13c93dfe5807161c6c936ac791fdc6344ed336198d8003ea3ff3ad0e6`  
		Last Modified: Thu, 22 Oct 2020 08:22:50 GMT  
		Size: 7.4 KB (7357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a56ef7489285b5bf73458a0ef468bc8cb5da5c162e07a83db24eefe8309e1c7`  
		Last Modified: Thu, 22 Oct 2020 08:22:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c697bf3717615851613ec8206bb233eec026608f7ce7ca7d93928d46fb8b5c`  
		Last Modified: Thu, 22 Oct 2020 08:22:51 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd12db22a23a011fc78203f0f4dbbbd5090d7f9f681da7e4351bc7aa47efa87`  
		Last Modified: Thu, 22 Oct 2020 08:22:50 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58b5a7c73c1b4fae5f6282219ca90da7beb6dcb82da335f7b7d20c339c57427`  
		Last Modified: Thu, 22 Oct 2020 08:22:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:609991c0b7f1a59a2155bed83915225177d0fdd3894bbb21c6b8f6d583b62b61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27487312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49cfae1a7604e03746aca74d6fc42d2f8d073bcc62a594e671bbd6cbed6d59d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:55:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:55:00 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:55:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:09:37 GMT
ENV PG_MAJOR=10
# Thu, 22 Oct 2020 09:09:38 GMT
ENV PG_VERSION=10.14
# Thu, 22 Oct 2020 09:09:38 GMT
ENV PG_SHA256=381cd8f491d8f77db2f4326974542a50095b5fa7709f24d7c5b760be2518b23b
# Thu, 22 Oct 2020 09:12:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:12:31 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:12:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:12:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:12:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:12:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:12:39 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:12:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:12:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:12:42 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:12:43 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:12:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54bc8a79538fa79db3e734327f2a73654bc80285dc55b7e4d8d206161ec79a9`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30574d1822b9e42c2a6da5e4a8f52ab65d88be941e497b4565382967ebd326f8`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6a0e93a2fea389b04769d0eecda70c6edeabeb89dc769053632f8bb98763f9`  
		Last Modified: Thu, 22 Oct 2020 09:20:52 GMT  
		Size: 24.9 MB (24871886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f16a189a70252e30be0d1b6407d31c24f3fe3a4d09f888e117720826226162`  
		Last Modified: Thu, 22 Oct 2020 09:20:42 GMT  
		Size: 7.4 KB (7353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161d5bb0709ab520bb7c41056869abe9cefe26873452da2d462369ae2b609ca1`  
		Last Modified: Thu, 22 Oct 2020 09:20:42 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfe9de5027701f4db18832991ab133fa4096b978ec27bb6dc1ba485de6759f0`  
		Last Modified: Thu, 22 Oct 2020 09:20:42 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2ecce049f4bf8fcf2fa890775a8e1cf79d55167eedd3993844aa82628d9f20`  
		Last Modified: Thu, 22 Oct 2020 09:20:41 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdb4ab64ed3d87328f97c2660bc1dd92fed1ed33eef6e7f1fe6e2519f795aea`  
		Last Modified: Thu, 22 Oct 2020 09:20:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:ab0003d8379a834b47d81e5fec211f4ad9cfcfde0e33f9e0956ecf583c222899
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26431645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d08bdce52318c18890b229f3883f479e2b66555044010f57df38a3375598db6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:56:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:56:03 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:56:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:07:48 GMT
ENV PG_MAJOR=10
# Thu, 22 Oct 2020 09:07:48 GMT
ENV PG_VERSION=10.14
# Thu, 22 Oct 2020 09:07:49 GMT
ENV PG_SHA256=381cd8f491d8f77db2f4326974542a50095b5fa7709f24d7c5b760be2518b23b
# Thu, 22 Oct 2020 09:10:05 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:10:08 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:10:10 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:10:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:10:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:10:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:10:15 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:10:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:10:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:10:19 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:10:20 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:10:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7eedf40b1ca3ca0c12781ef9399626d49e7898eb4dc6bf3888a3add86c9ee2`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2cc4a27e16f2350721162545664e1c967b92e8a0ecffb90828c979f0bc3ac6`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760a4aace192bdec6bc1847c2f3ef674a4abaec4fafae76061cb5ec6f84ece7d`  
		Last Modified: Thu, 22 Oct 2020 09:18:36 GMT  
		Size: 24.0 MB (24012456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44451f057148b5e725bb0f5d441a875a68932687363b4080a15266aba05b134`  
		Last Modified: Thu, 22 Oct 2020 09:18:26 GMT  
		Size: 7.4 KB (7351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9983d94b724a7572c00318fb2d5a97b9720522b5bd59baec657178b863bf9f5`  
		Last Modified: Thu, 22 Oct 2020 09:18:27 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b8c506bfd0757ab00eaa8ca6a918876b418f8591b60d2252704e67dd3d15ff`  
		Last Modified: Thu, 22 Oct 2020 09:18:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e859a013646c5293bd3426e306f94207520d7c01f25099ff142cffc8d66abd6`  
		Last Modified: Thu, 22 Oct 2020 09:18:26 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84cea1ff41bc00d3ccad455031e75bc06072c9b84a2404b0bcf6db05ef897ed`  
		Last Modified: Thu, 22 Oct 2020 09:18:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:71fceec91117bf0c08f9dc6ea88f2e18b6d09c454096999986226e3a996a3eb6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.2 MB (28155543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a90eab46892b4981cb0eb56d2776cc555acf6dd877389117befd5c380b00f6f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:21:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:21:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:21:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:34:09 GMT
ENV PG_MAJOR=10
# Thu, 22 Oct 2020 08:34:10 GMT
ENV PG_VERSION=10.14
# Thu, 22 Oct 2020 08:34:11 GMT
ENV PG_SHA256=381cd8f491d8f77db2f4326974542a50095b5fa7709f24d7c5b760be2518b23b
# Thu, 22 Oct 2020 08:36:42 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:36:45 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:36:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:36:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:36:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:36:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:36:53 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:36:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:36:58 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:36:59 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:37:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b3b77440641e62ecc741cdb44f0f558d15c3f3b6d506be26f8c285f7a36ff`  
		Last Modified: Thu, 22 Oct 2020 08:44:00 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85615d5b5e22de086f665265885eae6f4cb41a63e5ed6910df6d0d03d0e90c5`  
		Last Modified: Thu, 22 Oct 2020 08:43:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8df619139d08cf9322d74f01072ee2ee2cc9dd3e6b624e995591899326457f`  
		Last Modified: Thu, 22 Oct 2020 08:45:23 GMT  
		Size: 25.4 MB (25435469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48ffc8a58e9994b732a5efb88eba5b56e1a31ae619829cc117895caf8e65c1b`  
		Last Modified: Thu, 22 Oct 2020 08:45:15 GMT  
		Size: 7.4 KB (7355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e5e849338bf7d410d30f193b5866e8a129cb812f23825e5168d3bd22407852`  
		Last Modified: Thu, 22 Oct 2020 08:45:15 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2897d697b650e56672c460bc85ed6b32a7e644d7ae0b7fc244bb0980d5a4d398`  
		Last Modified: Thu, 22 Oct 2020 08:45:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6131bbf6ccf32c6c9790f84e5ceef0881e1aab53f56e5769d6d83e07c333f4b`  
		Last Modified: Thu, 22 Oct 2020 08:45:15 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7048a149a73da080436b33d9e3be25bd453c91b396640e69d1614a33f9ea51`  
		Last Modified: Thu, 22 Oct 2020 08:45:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; 386

```console
$ docker pull postgres@sha256:2a9741df36910532754196d260b5cdba46637ff94020fe6982b6ef4e615159a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29302512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d0d28eabf540959f1f08a93285acd295bd2185b1e159434a15d287a7a2d1028`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:38:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:38:39 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:38:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 10:05:29 GMT
ENV PG_MAJOR=10
# Thu, 22 Oct 2020 10:05:30 GMT
ENV PG_VERSION=10.14
# Thu, 22 Oct 2020 10:05:30 GMT
ENV PG_SHA256=381cd8f491d8f77db2f4326974542a50095b5fa7709f24d7c5b760be2518b23b
# Thu, 22 Oct 2020 10:10:34 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 10:10:35 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 10:10:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 10:10:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 10:10:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 10:10:36 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 10:10:37 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 10:10:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 10:10:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 10:10:38 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 10:10:38 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 10:10:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596122efb908f979efd1794c09ae9c7a15ac0e4d53f2c181fd646d9f32565d9a`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeb7bd791d51cd161cadd22b53bd066e70998ebd55dd5ba92760d35f1ab9e8b`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d6cbea72cc921131a0269de69a3df09568719f4e06b855c1a8b16de886c5dc`  
		Last Modified: Thu, 22 Oct 2020 10:22:21 GMT  
		Size: 26.5 MB (26497716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095e96855464c4888f18f9416f89ebac1c2e0aecf3d599ce6fa3e2c87e55890c`  
		Last Modified: Thu, 22 Oct 2020 10:22:11 GMT  
		Size: 7.4 KB (7351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288e80c4e4e820335de46e9fdb050ef1e9db80b264f2cddae65002be1efcdcc`  
		Last Modified: Thu, 22 Oct 2020 10:22:11 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4517033ba3de6835de6a0c66a9871a170b08dfe06b4b610ffecdf083e2e5184d`  
		Last Modified: Thu, 22 Oct 2020 10:22:11 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b88e3b1cd907ef63c7700d32fcc31596f4ae49a3d3d14715d7f5d8a8cf4a9d8`  
		Last Modified: Thu, 22 Oct 2020 10:22:11 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1a69c91e5a22ff44c4f82f421d2ac80cbc5349cc796b5cb3f548cfb3dbdbf3`  
		Last Modified: Thu, 22 Oct 2020 10:22:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:d3f4cecf04d31854afc9bf2e411c7a9256e5a5bf6e31d57e4d97a1ac2812473f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29548149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed3aadb24b17ff39ca7e8c823b096cd7092ff5f1b8de9822aadf064897eeaf42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 23:06:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 23:06:17 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 23:06:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 23:26:15 GMT
ENV PG_MAJOR=10
# Thu, 22 Oct 2020 23:26:26 GMT
ENV PG_VERSION=10.14
# Thu, 22 Oct 2020 23:26:33 GMT
ENV PG_SHA256=381cd8f491d8f77db2f4326974542a50095b5fa7709f24d7c5b760be2518b23b
# Thu, 22 Oct 2020 23:30:01 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 23:30:18 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 23:30:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 23:30:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 23:31:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 23:31:08 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 23:31:12 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 23:31:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 23:31:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 23:31:37 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 23:31:42 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 23:31:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cba28bb2e7e5449306ade2eb73dd95379370b59f2eac45aa9f62aa4d376b1`  
		Last Modified: Thu, 22 Oct 2020 23:41:44 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b145001d871735701a01931a308a05fafba12a34115cac00163359d3ed8cf19`  
		Last Modified: Thu, 22 Oct 2020 23:41:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b45355b16f038881cabffb1db3a781d2d62a85edd6ef0f461f2cca702a0f404`  
		Last Modified: Thu, 22 Oct 2020 23:43:38 GMT  
		Size: 26.7 MB (26731415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f7f64eae7981e3d2eb56251fe92b2b8dea6430c7e1ad753258d9a264ed4738`  
		Last Modified: Thu, 22 Oct 2020 23:43:26 GMT  
		Size: 7.4 KB (7353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1faeaf735e905689e3cd0625883234eab8c32ec8dda1b145a332a3115772725`  
		Last Modified: Thu, 22 Oct 2020 23:43:27 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfa457b2539c4a85db89b7979c4ccd694f52693cba954941a0aaa79d4fb4e74`  
		Last Modified: Thu, 22 Oct 2020 23:43:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c4195c3ca747d59689f002aa21f562626a7b2109255a8a97cae0d7c57497dc`  
		Last Modified: Thu, 22 Oct 2020 23:43:26 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8cfaa5076cc6242fdc433c8a6f0b9f1a612a77496c2609a744e7e43d6be21f`  
		Last Modified: Thu, 22 Oct 2020 23:43:27 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:94331878090fb64e847857d2f9f53e210e6e57179a5d7b4f5c8e0a099e7976fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28146984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221a15bcfbc64547c4884d9be9989f3e1b63b422cbdef5908b72b59d1e0f2b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:05:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:05:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:05:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:20:01 GMT
ENV PG_MAJOR=10
# Thu, 22 Oct 2020 09:20:01 GMT
ENV PG_VERSION=10.14
# Thu, 22 Oct 2020 09:20:02 GMT
ENV PG_SHA256=381cd8f491d8f77db2f4326974542a50095b5fa7709f24d7c5b760be2518b23b
# Thu, 22 Oct 2020 09:22:49 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:22:54 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:22:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:22:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:22:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:22:57 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:22:58 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:22:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:23:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:23:01 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:23:01 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:23:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788b366e4c5d5f3b69b31ae06b2811fe54eb39bd4fd8b6107985f9982ab150a`  
		Last Modified: Thu, 22 Oct 2020 09:29:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eed686015d5efd53e62cc5b3f61833711a48184edf03c7d21f021b34f23095`  
		Last Modified: Thu, 22 Oct 2020 09:29:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c568d7b10fb31f112471ff9e4d434cec4ce52e29b3e7d7ac2e4b06eeea10ad5`  
		Last Modified: Thu, 22 Oct 2020 09:30:28 GMT  
		Size: 25.6 MB (25567648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6044557b4cf946fc9a3f228a9c54430cf7029c0ce19a7e8d4dc13c0afc10e26`  
		Last Modified: Thu, 22 Oct 2020 09:30:22 GMT  
		Size: 7.3 KB (7347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057665bc4a30010d0de8101b218a2d76400678e5b95a2fa43d9eaf36d25af074`  
		Last Modified: Thu, 22 Oct 2020 09:30:22 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e53c41c5a3878f08eb3e30e255593bbe9aee068c2ae0ef0bfe997b71dd6000`  
		Last Modified: Thu, 22 Oct 2020 09:30:22 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605fefab79f089f68a91ab2f4f71051736ea7a311f43b8df96c54fd8926b62ae`  
		Last Modified: Thu, 22 Oct 2020 09:30:22 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c860b52f7ef8857e151f651de964b5888e3e9764fc0ea3d1892c411dd0f8fae3`  
		Last Modified: Thu, 22 Oct 2020 09:30:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:11`

```console
$ docker pull postgres@sha256:d441bf645a1dcd2b4429d916c276d4c01299ee16b7a0e0f3d0baa846cbd4ee07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:11` - linux; amd64

```console
$ docker pull postgres@sha256:72be9fbaa43eabe2200913cebddf3a8532f8eead1935a1f8707f65ad0c95771e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.4 MB (106428182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e07f0c129d9a26cee91d34a544ec2d00e8b3f4eb45a70cdaef2e466e51eefe59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:33:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:33:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:33:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:33:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:34:01 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:34:02 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:34:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:34:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:34:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:34:15 GMT
ENV PG_MAJOR=11
# Tue, 13 Oct 2020 12:34:15 GMT
ENV PG_VERSION=11.9-1.pgdg90+1
# Tue, 13 Oct 2020 12:34:48 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:34:49 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:34:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:34:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 13 Oct 2020 12:34:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:34:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:34:53 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:34:54 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:34:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:34:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:34:56 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:34:56 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:34:57 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0526c44df6ea5bd7668eab6d9c37d43aef6474cb4f5b6d2539e82404a3827041`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 4.5 MB (4502050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2466ee00e96ac149c287cdd533cecad2907d0aea2f2fe5ffc7a706ab313aaac`  
		Last Modified: Tue, 13 Oct 2020 12:38:27 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c605d60192c83f6a890b4f0cfaf8d80cf2a7a5c0c8df01451a106305748bf2`  
		Last Modified: Tue, 13 Oct 2020 12:38:28 GMT  
		Size: 1.4 MB (1412112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b14ab418421f0d1e9fb147720201f216050e2ad983640a446e75249e84e9bc`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 6.2 MB (6182797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f557fff31511f1f9475342998e8b195c0942480fb4901dab214f015d2224c`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 384.9 KB (384916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bba27806f46c2448fe4d5a0b248fd9178ced6163b8e2154e4b06a86c9a08b4`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e1555090548b1ab5739971b4eea16b502cc1e625f3a0b827463c4ae69bcc61`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb8e47accdf7db28e8881368a209651b2fdde1b8517cfbfecb02e0e56fb3cd6`  
		Last Modified: Tue, 13 Oct 2020 12:38:44 GMT  
		Size: 71.4 MB (71404017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de89dffa0b49dd2db32a8b25c9cfd5b47a9669ce366459b597bb04d74b922136`  
		Last Modified: Tue, 13 Oct 2020 12:38:25 GMT  
		Size: 8.3 KB (8268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7294df4e253d20d9f10366dd0a89d493305caa434fe1af85be53f0e9ed1262`  
		Last Modified: Tue, 13 Oct 2020 12:38:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddd01426f4ae0459295e18f45b596080b872742e279f62c0e2c089dc0ebcc8a`  
		Last Modified: Tue, 13 Oct 2020 12:38:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b846471366bfc0f47e6b7353314657de7eb03974aa41e50d517b19ac3254b48f`  
		Last Modified: Tue, 13 Oct 2020 12:38:25 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee58835750141237762f08cb246bb19c425a937570e85a550446df911d04cb2d`  
		Last Modified: Tue, 13 Oct 2020 12:38:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; arm variant v5

```console
$ docker pull postgres@sha256:72d1afa331333d7560345237118147a223d4985bd78fc5b445507776a9f45388
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70555602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a27272badf480fd2c978e2305c70e402bb482c20a09a2823c11519416acbb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:57:28 GMT
ADD file:ef761876435f34dd5e73f6fb89eda5cee26b26d9183a37dc5588c6eb5fd4ba69 in / 
# Tue, 13 Oct 2020 01:57:29 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 07:10:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 07:10:23 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 07:10:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 07:11:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 07:11:15 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 07:11:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:11:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 07:11:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 07:11:35 GMT
ENV PG_MAJOR=11
# Tue, 13 Oct 2020 07:11:36 GMT
ENV PG_VERSION=11.9-1.pgdg90+1
# Tue, 13 Oct 2020 07:33:02 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 07:33:05 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 07:33:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 07:33:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 13 Oct 2020 07:33:15 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 07:33:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 07:33:26 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 07:33:28 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:33:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 07:33:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:33:40 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 07:33:41 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 07:33:41 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e6fa5ab8c49c07aa49f655f00f7742fc2640bec642d3e0b440a9d67c37d1383e`  
		Last Modified: Tue, 13 Oct 2020 02:05:36 GMT  
		Size: 21.2 MB (21194476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4a7d58f9de066b4eb914552800ca9b9c3bdbd3a49d22592a568fd65353b60e`  
		Last Modified: Tue, 13 Oct 2020 08:37:11 GMT  
		Size: 4.2 MB (4238677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d9d67c7f2447a0677783317716fd66e891874c5dec4c300963bdaedef3db73`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8dfd96a4ee2041e6cf18fbfb05eaaf56b746f396297762c746643158da072a`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.4 MB (1371374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55137faf878bb43f0e314a0845bb679c3834709fb30668a8a966d3ea7d6324c6`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 6.2 MB (6185655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c626e10cc735d164b870d78d396556ebae2e833924a9782fc8880333228fea`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 385.1 KB (385110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5193a2411b31608c76d06bf9efa210a7cf0d1b51953e39d3cdc458342b259a86`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71923a948044364e5093b7b7e4e2667ee46f8e6fc34ff01d72050cd7aefbe702`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 5.3 KB (5350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8b09d6ba37ad824c97715ea9bd1392ab4d0276e2ebf6e3f24fabfae0c8344e`  
		Last Modified: Tue, 13 Oct 2020 08:37:20 GMT  
		Size: 37.2 MB (37160015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920d67a53baa9620d6838994f90a867c5953009f020f40006323848045f36f3f`  
		Last Modified: Tue, 13 Oct 2020 08:37:05 GMT  
		Size: 8.3 KB (8272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084191768f1bd604c7af5d0c81bae512a6af158f6204155176d7d25bb2c8406c`  
		Last Modified: Tue, 13 Oct 2020 08:37:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fedb73eba04446655e0f14cd75630bbe4d76fc0aca0a92c761cba5fbb567318`  
		Last Modified: Tue, 13 Oct 2020 08:37:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456c684e1e77bb22e81a12113cce789ac9fd0e7c5e1bb13bd7dd102f9a9f04c6`  
		Last Modified: Tue, 13 Oct 2020 08:37:05 GMT  
		Size: 4.3 KB (4267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3477bb86ad6e5691c88b1a7bf1155ee87fe9f6db52451786d20030bd399276`  
		Last Modified: Tue, 13 Oct 2020 08:37:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; arm variant v7

```console
$ docker pull postgres@sha256:47bd07df524d4aae55573af2b8de4c54e6b226d0f3f2db62adffad0f5a35ad62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67210075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11ff01a363eb5791cf057cae575cbc60e3a2319fb58400303addfc36073a78c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:04:30 GMT
ADD file:d204a257433edcd6f9ddd2c769b9e187c408eb4972203a5daab60214b5b576bc in / 
# Tue, 13 Oct 2020 01:04:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:54:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:54:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:54:44 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:55:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:55:24 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:55:25 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:55:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:55:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:55:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 05:55:47 GMT
ENV PG_MAJOR=11
# Tue, 13 Oct 2020 05:55:48 GMT
ENV PG_VERSION=11.9-1.pgdg90+1
# Tue, 13 Oct 2020 06:13:46 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 06:13:52 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 06:13:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 06:13:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 13 Oct 2020 06:13:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 06:13:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 06:13:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 06:14:00 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:14:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 06:14:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:14:05 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 06:14:06 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 06:14:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cc11be355171b10881b3ed16be16ceb2d7787cd459c6489d83bac55ee5824b35`  
		Last Modified: Tue, 13 Oct 2020 01:12:46 GMT  
		Size: 19.3 MB (19304540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8b70af887483c86f21ffd35a2a331fbab0ae0804a4929517360da6207fe6c3`  
		Last Modified: Tue, 13 Oct 2020 07:09:01 GMT  
		Size: 3.9 MB (3874946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09233e1347145a65db2aae548df648e91df34bde91664ac04509ff8ba2d77447`  
		Last Modified: Tue, 13 Oct 2020 07:08:59 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a09c7350562aee4559820b5fa1133618b8c02e7848e0c14635fb483b5a10fb`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 1.4 MB (1363819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9deba20fbd610072e97a51ac7766bcfdac37c6110ee53cdf296e7435868b5e7`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 6.2 MB (6185495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a750e8984fdec76cc5aa76a7979cd403c03d5b18efe690ebda5984356654554`  
		Last Modified: Tue, 13 Oct 2020 07:08:58 GMT  
		Size: 379.2 KB (379196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bd92fced2d524fc75c7429ca11a3f1c30587399ca0a571b4f623a3db6c15c2`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059b3634dc4169b9d362c9bf8d29e4c9af7a58bd40538452efeb506841942fb4`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad4d14efa6ace569bbe56210f6b4d67a1df40962402efc1880bd41b31b8bc49`  
		Last Modified: Tue, 13 Oct 2020 07:09:11 GMT  
		Size: 36.1 MB (36081783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1816a14ad9850521418f67990dff62d6fab1da31785ce667b4f764721da71d7d`  
		Last Modified: Tue, 13 Oct 2020 07:08:56 GMT  
		Size: 8.3 KB (8269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d295a2bfadc6b5766fdedff4ab60488344999ac5309af1731ef8113d2ea4f8a9`  
		Last Modified: Tue, 13 Oct 2020 07:08:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670f9ef6e487c16497956caed6328eacfc62fd7bdc5fbf821b2b2bf4e190b100`  
		Last Modified: Tue, 13 Oct 2020 07:08:56 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9264677ff785f2acaab94a8f33c1ef3b129c418eefd6ddc0356d96bba23386`  
		Last Modified: Tue, 13 Oct 2020 07:08:56 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed3bb8609e2abbeea75fe226faaafd0d5a7c3a444299e12e326815c14c5d38`  
		Last Modified: Tue, 13 Oct 2020 07:08:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:6821f66347e28c8ad391b436da22c01ea45f19d58b6aeb1550fb17acbdbc1fe3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69835439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6c19642d7d23b5b0a22918686aca03d7bf0086874bd3050c8639307433a99eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:21 GMT
ADD file:1783101ec41dba711940487fb45a9287f74a0639658051ad8bc9b2618a15be61 in / 
# Tue, 13 Oct 2020 01:44:22 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:04:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 11:04:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 11:04:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 11:04:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 11:05:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 11:05:06 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 11:05:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:05:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 11:05:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 11:05:22 GMT
ENV PG_MAJOR=11
# Tue, 13 Oct 2020 11:05:23 GMT
ENV PG_VERSION=11.9-1.pgdg90+1
# Tue, 13 Oct 2020 11:23:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 11:23:18 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 11:23:20 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 11:23:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 13 Oct 2020 11:23:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 11:23:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 11:23:25 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 11:23:25 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 11:23:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 11:23:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 11:23:29 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 11:23:30 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 11:23:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f4bec48cdb322f1180477bdd362bcd92d70a1ab628fc36319017bf4e8058d9ee`  
		Last Modified: Tue, 13 Oct 2020 01:51:12 GMT  
		Size: 20.4 MB (20376997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984be4b3fed9808b066a7600d2e83efbfd0ff4bfc1069a9d0814be2fd022f357`  
		Last Modified: Tue, 13 Oct 2020 12:20:59 GMT  
		Size: 4.1 MB (4078528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859bbaaf4e29eade0fbd81b43a64e5eb25198a55ef466f821ac3ba984a0bab4`  
		Last Modified: Tue, 13 Oct 2020 12:20:57 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882cfdcc3440ef89e60ecc554c9e53baa9bbbc241e2b37005dcd3d8f1faabdc9`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 1.3 MB (1346994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a8ef2ba5300bad73627e9166d141b0a67a7ad8d42cb3453893fb5f5813dea`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 6.2 MB (6185301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652a08bb6feda1aad8370161437fc26c9908787e595304676ceb34feafbbe901`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 377.9 KB (377937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17111fdbd30125a36e0c8429df7d3ff1c54dfe90c2c0999e2f3738dc89019f00`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed1a1a2b06a19d02a8d4d5890f949a8a250c418de647be680f045f2240fd2e3`  
		Last Modified: Tue, 13 Oct 2020 12:20:51 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dca707007010fd2e53b3771e2d9e24d9dc9dfd51b182a144a8faedde291b200`  
		Last Modified: Tue, 13 Oct 2020 12:21:03 GMT  
		Size: 37.4 MB (37449384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4857cc01fa67c93077621654e0157c755f20baad500d2ea60654723cdb256134`  
		Last Modified: Tue, 13 Oct 2020 12:20:49 GMT  
		Size: 8.3 KB (8272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedfd662e3998cf4ecf7cc16df391d24c0ede76a931a2acfa8fc28322c0acd22`  
		Last Modified: Tue, 13 Oct 2020 12:20:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6206051f15bdfa6acec7f76ff5675d314c1d616ab657e30a079c5f25bba1d89`  
		Last Modified: Tue, 13 Oct 2020 12:20:49 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414a0573d5a5cc9cdf45901974aa9de7118ec7b5c6f9d179d9ad6076ed7af93d`  
		Last Modified: Tue, 13 Oct 2020 12:20:49 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5eeaaa770b68e8406542c4ee961cbce33a58130e3f31f00758f774ae85793f`  
		Last Modified: Tue, 13 Oct 2020 12:20:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11` - linux; 386

```console
$ docker pull postgres@sha256:38f58c400dc1bfd7467432b9c854bbd83bafe6864aeff9c54edffa267498acf2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109875240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae3b776aad8ecf3fd73c939c21667de98417c19a9b858a680ae2aa8cc6d3804`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:45:31 GMT
ADD file:f09276bb607e6d68dcb997c1e8b4d004b91548964306d6a803286ba851484579 in / 
# Tue, 13 Oct 2020 01:45:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 16:43:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 16:43:18 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 16:43:18 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 16:43:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 16:43:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 16:43:49 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 16:43:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:43:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 16:44:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 16:44:03 GMT
ENV PG_MAJOR=11
# Tue, 13 Oct 2020 16:44:03 GMT
ENV PG_VERSION=11.9-1.pgdg90+1
# Tue, 13 Oct 2020 16:44:31 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 16:44:32 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 16:44:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 16:44:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 13 Oct 2020 16:44:34 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 16:44:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 16:44:36 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 16:44:36 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 16:44:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 16:44:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 16:44:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 16:44:39 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 16:44:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:02448e4a5fa68035acff67a00ba04305cbad42b25ffeb4b141c5f1f0b9d63a2a`  
		Last Modified: Tue, 13 Oct 2020 01:52:11 GMT  
		Size: 23.1 MB (23148149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1707623e5e9b92a3f43f1910a43ad9872060b853d07ecbf2b9b5bc02300501`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 4.8 MB (4809899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7908ca805e2bd89c5f1fe55e4f313469b7d84f6d049e59bc673439f8323b1d`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebde576b2c220dc444db8fcec0278f11a1df5bce6d091728aa378f74bb22734e`  
		Last Modified: Tue, 13 Oct 2020 16:48:40 GMT  
		Size: 1.4 MB (1382391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f9c2ca0b45e9e11f84e7f98ba02d277d65687fd873580517a5f0e50e6d7aac`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 6.2 MB (6182990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd5fdfe0405da8b45de435a650073673e910b7bd9545f2a05811eed28824401`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 393.2 KB (393233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3263197a4dd54e9fefd6e411e83b19f4186837e5aa15ce30c389245a5f7ae727`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1249d81ef1b333d5c1caf34a641e9466c3351724f2e669c983df59e95e4571`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9effbafafd0d60651282c58aa017671a20cac50b57c59a9cf4478c9bbdd66a72`  
		Last Modified: Tue, 13 Oct 2020 16:49:12 GMT  
		Size: 73.9 MB (73938388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161a019bdee3315a31cdf6276c71e9bbd36107e9c2551d746e195b48fdce271f`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 8.3 KB (8271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c436fa9e6aaff209375167e008a2a9b91c00f758d5b29d792faef9f870b1b59`  
		Last Modified: Tue, 13 Oct 2020 16:48:37 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bb469af92ac11fe4cc3b901fa4c0fcdb07558a92340b3dd90f73211737c022`  
		Last Modified: Tue, 13 Oct 2020 16:48:37 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fced6e717cf4b24f8eaae7b387864f771dfbb2af89efba4b3ed09b16feb05f`  
		Last Modified: Tue, 13 Oct 2020 16:48:37 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23508a39bf70a49bd51bd0c4f8401cff501725a13265df167ce869f845bef0a5`  
		Last Modified: Tue, 13 Oct 2020 16:48:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:11.10`

**does not exist** (yet?)

## `postgres:11.10-alpine`

**does not exist** (yet?)

## `postgres:11-alpine`

```console
$ docker pull postgres@sha256:b57ab77e7888c37a8ad064fb45a8d8a88bde7151d2b889f88a807d4194756397
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
$ docker pull postgres@sha256:d90bdb72921e546c95d5562a4d8c6ae9db2a9bd5fe09be75e44fb1b9ac3b26d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60284743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b6cc286aa5cd9b86bc66905f1b2c2a250ceac3651e4e7ea9d280ffa9b6a511`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:55:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 07:55:14 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 07:55:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:06:44 GMT
ENV PG_MAJOR=11
# Thu, 22 Oct 2020 08:06:44 GMT
ENV PG_VERSION=11.9
# Thu, 22 Oct 2020 08:06:44 GMT
ENV PG_SHA256=35618aa72e0372091f923c42389c6febd07513157b4fbb9408371706afbb6635
# Thu, 22 Oct 2020 08:11:59 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:12:00 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:12:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:12:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:12:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:12:02 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:12:02 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:12:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:12:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:12:03 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:12:03 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:12:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f1d1b70e7fa650fd6229086120f763219adce9e33e8b20bdfbf8452ab69847`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4f01476d2b86761cdb0414c4a583b89af3b5d0b67022cfc0d378743307f7e3`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d058ff3c2e76b5b2b73fe978d13098a08147a1ab7a3626aaf9ad2a517063ac4d`  
		Last Modified: Thu, 22 Oct 2020 08:22:45 GMT  
		Size: 57.5 MB (57474273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78813ef71e2f8248d9cef38ce7fe0eca079e0e68c4c583d6260740ae187581a`  
		Last Modified: Thu, 22 Oct 2020 08:22:34 GMT  
		Size: 7.6 KB (7568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995bee851f84b1ea98efd4d182c4e647ff1130f196ca28f21cf85c910549ff1b`  
		Last Modified: Thu, 22 Oct 2020 08:22:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09fcc1822869a254dbc7ef4f85dbecb2221d373edfe1510d7a7bd89b43d4507`  
		Last Modified: Thu, 22 Oct 2020 08:22:34 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779826b7296000ccf24486a5877f8f0f55a7f3bc61fa1d3549b4ca43c12d7bed`  
		Last Modified: Thu, 22 Oct 2020 08:22:34 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7019d6614cc2989650b8c2d6c20716e6bb45b449f457c92c71e1fc7157d9161c`  
		Last Modified: Thu, 22 Oct 2020 08:22:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:8192eab3bf1a5f53f530cdea61c0204a92e2d57d389a60f3334946c4ec822b7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.5 MB (58480791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99fd90a415e7bcad3ee1ad586d2ca79d88ceb9a1488a902a119a0d45ad0e1b00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:55:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:55:00 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:55:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:04:59 GMT
ENV PG_MAJOR=11
# Thu, 22 Oct 2020 09:05:00 GMT
ENV PG_VERSION=11.9
# Thu, 22 Oct 2020 09:05:02 GMT
ENV PG_SHA256=35618aa72e0372091f923c42389c6febd07513157b4fbb9408371706afbb6635
# Thu, 22 Oct 2020 09:09:13 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:09:16 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:09:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:09:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:09:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:09:21 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:09:21 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:09:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:09:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:09:24 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:09:25 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:09:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54bc8a79538fa79db3e734327f2a73654bc80285dc55b7e4d8d206161ec79a9`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30574d1822b9e42c2a6da5e4a8f52ab65d88be941e497b4565382967ebd326f8`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c75827a5b01990441c306c995d7fcda9425c0bade77bbf0c66825580af0273`  
		Last Modified: Thu, 22 Oct 2020 09:20:33 GMT  
		Size: 55.9 MB (55865143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738b7fda4e13330b340ba0fbd9aa4911c7260abe0650464553a0010585f70c33`  
		Last Modified: Thu, 22 Oct 2020 09:20:12 GMT  
		Size: 7.6 KB (7571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3b5dd01c49e1c24b40bcdd9903fd8376ad5a564e53d4f1652917c90907533e`  
		Last Modified: Thu, 22 Oct 2020 09:20:13 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94dffc034c095018d0104caabd5eb6de495c82851ad8ea41d416e94ea4a3994`  
		Last Modified: Thu, 22 Oct 2020 09:20:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56588f7e97f957dc6dbe292261447a7f660b7275f367a710fcacde53926f8e4`  
		Last Modified: Thu, 22 Oct 2020 09:20:12 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8578c7dc3e8da1e729ad0ea6deb3919c7a835d131b1e30527e8cfd7c8c49125a`  
		Last Modified: Thu, 22 Oct 2020 09:20:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:ac3bf6bd9afb1e32d31d18edc45d29cd90e2a1a5fecbab858a756bfb2469cadd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55674782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bdac71f8334773ad13d2386db8ff595e506381740697c21c28e0c62189d8196`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:56:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:56:03 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:56:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:04:07 GMT
ENV PG_MAJOR=11
# Thu, 22 Oct 2020 09:04:08 GMT
ENV PG_VERSION=11.9
# Thu, 22 Oct 2020 09:04:09 GMT
ENV PG_SHA256=35618aa72e0372091f923c42389c6febd07513157b4fbb9408371706afbb6635
# Thu, 22 Oct 2020 09:07:17 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:07:20 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:07:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:07:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:07:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:07:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:07:27 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:07:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:07:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:07:30 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:07:30 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:07:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7eedf40b1ca3ca0c12781ef9399626d49e7898eb4dc6bf3888a3add86c9ee2`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2cc4a27e16f2350721162545664e1c967b92e8a0ecffb90828c979f0bc3ac6`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8744965d85a887a1a7a3dced6f0202ead4d55efa0b7588528f7735586c3b5683`  
		Last Modified: Thu, 22 Oct 2020 09:18:18 GMT  
		Size: 53.3 MB (53255369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a06383560e1db5eac489179766919bc67da0f176d9160c272b1146b7278e8d`  
		Last Modified: Thu, 22 Oct 2020 09:18:01 GMT  
		Size: 7.6 KB (7573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be62bea1696e58983b8d9c43c605c50a423c6bbc40813ab47fc5fb0d67a9cc5`  
		Last Modified: Thu, 22 Oct 2020 09:18:01 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d0d783ebbf14db0c1817b13cf9e9f9f9a7755c4621234da376fa849860282d`  
		Last Modified: Thu, 22 Oct 2020 09:18:01 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f2fe42f6b532ccae3c1aee2136e59777b73fcb03fae56366c0c14398bbdb2b`  
		Last Modified: Thu, 22 Oct 2020 09:18:01 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29147edddff1f66375d08dc6df6c1681e26699760f8e37dbae1ff786e5615d54`  
		Last Modified: Thu, 22 Oct 2020 09:18:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:3ab21a2131d6becdfbaeaae1988a8ce31a72205b48db98ee97edbf872691efb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.9 MB (59855172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f42ba4208d66ccfcd26e6eae35bc43f8e2c62b834f558f8774b873189fd7e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:21:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:21:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:21:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:30:28 GMT
ENV PG_MAJOR=11
# Thu, 22 Oct 2020 08:30:30 GMT
ENV PG_VERSION=11.9
# Thu, 22 Oct 2020 08:30:31 GMT
ENV PG_SHA256=35618aa72e0372091f923c42389c6febd07513157b4fbb9408371706afbb6635
# Thu, 22 Oct 2020 08:33:41 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:33:45 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:33:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:33:47 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:33:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:33:49 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:33:50 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:33:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:33:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:33:53 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:33:54 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:33:57 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b3b77440641e62ecc741cdb44f0f558d15c3f3b6d506be26f8c285f7a36ff`  
		Last Modified: Thu, 22 Oct 2020 08:44:00 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85615d5b5e22de086f665265885eae6f4cb41a63e5ed6910df6d0d03d0e90c5`  
		Last Modified: Thu, 22 Oct 2020 08:43:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e62537e567035c5999657615bd736409c64f41e942b3f87e615c66ae52a8cb`  
		Last Modified: Thu, 22 Oct 2020 08:45:03 GMT  
		Size: 57.1 MB (57134879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23fb5551ecc716a44734ad6358e1e78e7e79c98a3a9f96de760c29cb33890c5`  
		Last Modified: Thu, 22 Oct 2020 08:44:48 GMT  
		Size: 7.6 KB (7574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baa45aa7871810c573597f945354762e83b06811f6d056d0ab88464a510059b`  
		Last Modified: Thu, 22 Oct 2020 08:44:47 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4f31d3813ec635ab947d8920d2f5c647368804aaa6daf6534a2c760881cf88`  
		Last Modified: Thu, 22 Oct 2020 08:44:47 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57f6651ce34adfa7b1c188d1d9db8089308598f50a74690d4c7ece8abc5db`  
		Last Modified: Thu, 22 Oct 2020 08:44:47 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8953d6050ea0981260cd058299c4cdf3393cbec496c99879bd52cbcfb9702ae9`  
		Last Modified: Thu, 22 Oct 2020 08:44:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; 386

```console
$ docker pull postgres@sha256:246bdf2dbc76272797dcd41ad798196edca3d722bb513b62eb6103c294b77633
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63730172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:507448e29b66cd904c55c29e70c6bdebd64c70a706c2432fc0155d2e41b2f0d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:38:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:38:39 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:38:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:56:33 GMT
ENV PG_MAJOR=11
# Thu, 22 Oct 2020 09:56:33 GMT
ENV PG_VERSION=11.9
# Thu, 22 Oct 2020 09:56:33 GMT
ENV PG_SHA256=35618aa72e0372091f923c42389c6febd07513157b4fbb9408371706afbb6635
# Thu, 22 Oct 2020 10:05:14 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 10:05:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 10:05:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 10:05:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 10:05:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 10:05:17 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 10:05:17 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 10:05:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 10:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 10:05:18 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 10:05:18 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 10:05:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596122efb908f979efd1794c09ae9c7a15ac0e4d53f2c181fd646d9f32565d9a`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeb7bd791d51cd161cadd22b53bd066e70998ebd55dd5ba92760d35f1ab9e8b`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71596638f4cb5ee55cb116399fdb509d66c3149edddf1f094c943180fea0152b`  
		Last Modified: Thu, 22 Oct 2020 10:22:04 GMT  
		Size: 60.9 MB (60925160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3fbbc039d845be147cf1e8ade909c608fce49f780fc305499335342af47da3`  
		Last Modified: Thu, 22 Oct 2020 10:21:42 GMT  
		Size: 7.6 KB (7567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3286005b39b93266d34cf1832ade3eb57c05f145665df52bbef3ca0e2a0ed8cf`  
		Last Modified: Thu, 22 Oct 2020 10:21:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e598e131dae5e6c554323fe4a1e359fa80c0aced1efed1a3ddbd185cec28b0d4`  
		Last Modified: Thu, 22 Oct 2020 10:21:42 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e4b7f4fcd7fbb1c3422e9ab1130b63d9c872177a9b6baec8d0d75f7e4b81b1`  
		Last Modified: Thu, 22 Oct 2020 10:21:42 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3e67d5de4f44cadd77e74959c6283063ff9be8208dd89011b87431c5c0e165`  
		Last Modified: Thu, 22 Oct 2020 10:21:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:233f3c9b59e0ae1c4e5b66c91254f8eb2c3de433fca19ad52aa754cc977ff773
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62597918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d72cc9c6a06974116e8ef0985c17673d29ed961f253d5e109ec467717f7b6243`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 23:06:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 23:06:17 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 23:06:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 23:18:56 GMT
ENV PG_MAJOR=11
# Thu, 22 Oct 2020 23:19:01 GMT
ENV PG_VERSION=11.9
# Thu, 22 Oct 2020 23:19:07 GMT
ENV PG_SHA256=35618aa72e0372091f923c42389c6febd07513157b4fbb9408371706afbb6635
# Thu, 22 Oct 2020 23:23:53 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 23:24:19 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 23:24:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 23:24:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 23:25:01 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 23:25:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 23:25:12 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 23:25:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 23:25:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 23:25:39 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 23:25:43 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 23:25:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cba28bb2e7e5449306ade2eb73dd95379370b59f2eac45aa9f62aa4d376b1`  
		Last Modified: Thu, 22 Oct 2020 23:41:44 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b145001d871735701a01931a308a05fafba12a34115cac00163359d3ed8cf19`  
		Last Modified: Thu, 22 Oct 2020 23:41:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434f5cc8bd1952e121344b168a2a7e334ca70d490db66387ba551f2f1a4a2d48`  
		Last Modified: Thu, 22 Oct 2020 23:43:12 GMT  
		Size: 59.8 MB (59780961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0292c074ce16b8b026585acdebbb046b4901b84bc639e6ab8bd60371b52c8e5`  
		Last Modified: Thu, 22 Oct 2020 23:42:50 GMT  
		Size: 7.6 KB (7573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c719ad877f7f8fde18ac4f093c5bb10532b933c561c4c9742e9e0720c7dc70e`  
		Last Modified: Thu, 22 Oct 2020 23:42:49 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0a8304eb09715d642061745c5e3858c8f047dd0d122354d3e800b6dfc0f668`  
		Last Modified: Thu, 22 Oct 2020 23:42:49 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12379fdc1e3a797357d0406ab4c297be3e1f7d71ae8bce1a0cb80131ff87a8d1`  
		Last Modified: Thu, 22 Oct 2020 23:42:49 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0c39df09c3fe43f59cc37322b5b117a826e78f0e9c135bc11dfbd28e882b51`  
		Last Modified: Thu, 22 Oct 2020 23:42:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:093c2680e1f5145a6128454e53d300453d6268a96f9e8edc536ec34816d90c8a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62295324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e59cfb367565c5ae2807c62563c57f40bb412744449fc778dba37979caf02a98`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:05:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:05:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:05:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:15:07 GMT
ENV PG_MAJOR=11
# Thu, 22 Oct 2020 09:15:08 GMT
ENV PG_VERSION=11.9
# Thu, 22 Oct 2020 09:15:08 GMT
ENV PG_SHA256=35618aa72e0372091f923c42389c6febd07513157b4fbb9408371706afbb6635
# Thu, 22 Oct 2020 09:19:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:19:38 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:19:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:19:40 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:19:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:19:43 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:19:43 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:19:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:19:46 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:19:47 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:19:48 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788b366e4c5d5f3b69b31ae06b2811fe54eb39bd4fd8b6107985f9982ab150a`  
		Last Modified: Thu, 22 Oct 2020 09:29:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eed686015d5efd53e62cc5b3f61833711a48184edf03c7d21f021b34f23095`  
		Last Modified: Thu, 22 Oct 2020 09:29:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16148ba1fe81ee03e8fdbf5fb9ce5523b8798aaa9465d9a7ff5c0dd0533bffcc`  
		Last Modified: Thu, 22 Oct 2020 09:30:10 GMT  
		Size: 59.7 MB (59715761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51732098e722381869f1257190ef464936f5127a37b42c1695ce83fd1c33e919`  
		Last Modified: Thu, 22 Oct 2020 09:29:58 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9bcba9fb70dd7b486ce2c771b2d707722abb9cd18e06b94cdfd76c14c25b54`  
		Last Modified: Thu, 22 Oct 2020 09:29:58 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233a840c262bffce499df10f9f651527cd8f9fc8cbe0c74a3a8bd8ded5abe2c5`  
		Last Modified: Thu, 22 Oct 2020 09:29:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c546facf07eea426dca0daebf1c23549a916bf05fb8d8100c4d98b46ca2db4df`  
		Last Modified: Thu, 22 Oct 2020 09:29:59 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31dcd98b57d760807aed0fdbeae848a03ec906e47fa6340e62b4709c0b4f6e3`  
		Last Modified: Thu, 22 Oct 2020 09:29:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:12`

```console
$ docker pull postgres@sha256:a1e04460fdd3c338d6b65a2ab66b5aa2748eb18da3e55bcdc9ef17831ed3ad46
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

### `postgres:12` - linux; amd64

```console
$ docker pull postgres@sha256:c713cbd0e39ee3450bec6fa44e0f6236879b3dac79adc2d0417582785b8776b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114340139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:492fb9ae4e7af4e4aa4169afd0cc8738034f0abd313f231f5f607c067fff4654`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:31:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:31:49 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:31:49 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:31:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:32:06 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:32:07 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:32:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:32:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:32:13 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:32:49 GMT
ENV PG_MAJOR=12
# Tue, 13 Oct 2020 12:32:50 GMT
ENV PG_VERSION=12.4-1.pgdg100+1
# Tue, 13 Oct 2020 12:33:11 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:33:12 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:33:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:33:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 13 Oct 2020 12:33:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:33:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:33:14 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:33:14 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:33:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:33:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:33:15 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:33:16 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:33:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dc51fa2b560b7daf34aa4c2501941b4ce0d701c4ecf571777b13d79561f1bc`  
		Last Modified: Tue, 13 Oct 2020 12:37:32 GMT  
		Size: 4.2 MB (4178093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f213b6f96d81fa40e97b4eb61a159f716d77a4c70a25f376525385d7836bdee2`  
		Last Modified: Tue, 13 Oct 2020 12:37:31 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2780ac832fdea1b95491eaf082507289c13fc77e97de2716ee80e851cce0c79a`  
		Last Modified: Tue, 13 Oct 2020 12:37:31 GMT  
		Size: 1.4 MB (1419193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5cee1a3f123d23889bfdd0941b304d3906c90e136ec0e13f340b473096902f`  
		Last Modified: Tue, 13 Oct 2020 12:37:33 GMT  
		Size: 8.0 MB (7964517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95db3c06319e21f4c21eff545348f1755e5979d63c551a5b82bf9ff55ef30fa5`  
		Last Modified: Tue, 13 Oct 2020 12:37:30 GMT  
		Size: 391.1 KB (391050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475ca72764d52e2efe3b99160dbf36815c6be1ffda0790cc7e22354796185f08`  
		Last Modified: Tue, 13 Oct 2020 12:37:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d602872ecaeaf9c80cc4728578cc9a9b42d53b5f9351195a60f0be4455f99fd`  
		Last Modified: Tue, 13 Oct 2020 12:37:30 GMT  
		Size: 3.1 KB (3053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ed287c246e18a7a60d4ef10ff28954d85f237bdefddc4727100de1a66980a0`  
		Last Modified: Tue, 13 Oct 2020 12:38:20 GMT  
		Size: 73.3 MB (73276504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ff7d7e55c201d2d250a6505e2da62a19e66d8f52093c1be65b24b08aeb39ce`  
		Last Modified: Tue, 13 Oct 2020 12:37:52 GMT  
		Size: 8.9 KB (8938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecac36e2e8053ef8ac106e00a9139ce0aa78ac611ab167c3a6cb28fb72156760`  
		Last Modified: Tue, 13 Oct 2020 12:37:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c644377e015b73b249a3488a5dbcd6d539a121291cba9c2c199ee4fa9564a2d6`  
		Last Modified: Tue, 13 Oct 2020 12:37:51 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11db28dae1fe24378e4d630907514ed46a6a005284a38f2e8d156228460e080`  
		Last Modified: Tue, 13 Oct 2020 12:37:51 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b253e297b964f3a5fdea9c612dcef3f3958f0b935228b96f434244d5523f74`  
		Last Modified: Tue, 13 Oct 2020 12:37:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; arm variant v5

```console
$ docker pull postgres@sha256:59082a37ecec4f0d85fceaa84e42597b5186fe75a9bec4af2ebcbafa9394a43d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.6 MB (108613806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0272e55f9948e37c1eb7dbb2ebae28a3b09ff9a1dfc3312956928edd4d90eb2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:16:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 06:16:12 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 06:16:13 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 06:16:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 06:16:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 06:16:48 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 06:16:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:17:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 06:17:03 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 06:43:59 GMT
ENV PG_MAJOR=12
# Tue, 13 Oct 2020 06:44:00 GMT
ENV PG_VERSION=12.4-1.pgdg100+1
# Tue, 13 Oct 2020 07:09:40 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 07:09:46 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 07:09:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 07:09:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 13 Oct 2020 07:09:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 07:09:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 07:09:53 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 07:09:54 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:09:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 07:09:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:09:57 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 07:09:58 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 07:09:59 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220f749165a848f7f38bac836c52f4b835c99e7d95e05ee20dadaec192039226`  
		Last Modified: Tue, 13 Oct 2020 08:36:06 GMT  
		Size: 3.8 MB (3847907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99328c93a7de72d797aa8f54b8f5f65ac8dcfcb8adfcf619deb383521090b6a8`  
		Last Modified: Tue, 13 Oct 2020 08:36:05 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877588e4293d5c0bc10377dd6a2128f747be69e1e9176d0d8a2e6408917422ff`  
		Last Modified: Tue, 13 Oct 2020 08:36:05 GMT  
		Size: 1.4 MB (1378519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96f5e00aa670ea297c3d7b88aef48e3e83cecb4a2957ba6e1193fc4f3a0eba`  
		Last Modified: Tue, 13 Oct 2020 08:36:06 GMT  
		Size: 8.0 MB (7965207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e8a16e6b99574961ad43e457e425366fa1f111b3ce41c801ae3c66b5e68c86`  
		Last Modified: Tue, 13 Oct 2020 08:36:03 GMT  
		Size: 390.4 KB (390390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511e0945d4fb63b1f0366268b49f03e65681c8615d784c5ba2485563cf6d1f21`  
		Last Modified: Tue, 13 Oct 2020 08:36:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834364422035b3d7732f4346f19965cb41e38c4e33423185259f014337b1cfa0`  
		Last Modified: Tue, 13 Oct 2020 08:36:03 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d3514b5fd33f2c9cb895581a2259f4de5da9367e576ce082662d816de457c5`  
		Last Modified: Tue, 13 Oct 2020 08:36:57 GMT  
		Size: 70.2 MB (70177144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9b0bf8d5111d1382625df9300aece8461a87388e23370d2bd59b54d96a5a41`  
		Last Modified: Tue, 13 Oct 2020 08:36:33 GMT  
		Size: 8.9 KB (8937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5311daa42e38599f97a3d85cc3a9007ae2d62589da03bf6f9c0832a61e710dba`  
		Last Modified: Tue, 13 Oct 2020 08:36:34 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5b0699f2049e2b6a509763d848dddc289d5d5801c40c3b3821edef5c040dcb`  
		Last Modified: Tue, 13 Oct 2020 08:36:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb36ff1ffcde8ad397b7e934f289a8f475844bd7b2848b190007dcd5c7c1a5a2`  
		Last Modified: Tue, 13 Oct 2020 08:36:34 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa447c02e886bac5fd279cc37e516b9a0d7bf1c47bf4b4790f994b42290a596`  
		Last Modified: Tue, 13 Oct 2020 08:36:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; arm variant v7

```console
$ docker pull postgres@sha256:ebff946d43c6ed9d0571d85c622272a7996381dc91254dc0721c0230d3e2e623
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104669150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02913668dc2e1bfd4371efc4b9cfb246c55d38bc5d44b3325631f94292c375cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:03:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:03:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:03:10 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:03:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:03:51 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:03:52 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:04:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:04:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 05:29:46 GMT
ENV PG_MAJOR=12
# Tue, 13 Oct 2020 05:29:47 GMT
ENV PG_VERSION=12.4-1.pgdg100+1
# Tue, 13 Oct 2020 05:53:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 05:53:46 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 05:53:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 05:53:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 13 Oct 2020 05:53:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 05:53:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 05:53:57 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 05:53:58 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:54:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 05:54:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 05:54:04 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 05:54:05 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 05:54:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9abeb7fdbbade7b8abd012862e54cc393b34cd5ded22d30651c3d96f804017`  
		Last Modified: Tue, 13 Oct 2020 07:07:55 GMT  
		Size: 3.5 MB (3481628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c060aae45342f7e836211d989e2a8acbbc00aa77c9cedf463bc22d3931011b38`  
		Last Modified: Tue, 13 Oct 2020 07:07:54 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df78177be2b9c4f60b1d775bbe3774b00e3c1c567c4f122bbdff0d8c9be841a8`  
		Last Modified: Tue, 13 Oct 2020 07:07:54 GMT  
		Size: 1.4 MB (1370276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb71a60beb691d7f1f8351012f0a88049401c5ee2057e4a830758eee6c8dae4`  
		Last Modified: Tue, 13 Oct 2020 07:07:55 GMT  
		Size: 8.0 MB (7965243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3d3aab018a14d7c2ecdf71b6ba41d4a5521ba93a7a91a5ef2c466512f6165`  
		Last Modified: Tue, 13 Oct 2020 07:07:52 GMT  
		Size: 385.0 KB (385046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2443ca999a57081e3059a2ce066d226d974c0bfe22f8f887df06da48744d1b04`  
		Last Modified: Tue, 13 Oct 2020 07:07:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f35f400211e43d2986188ba441aee4ef58990df42a4f6215d473f4162cc97b5`  
		Last Modified: Tue, 13 Oct 2020 07:07:51 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f3f62b884b644d9abb068ac0fa302eeb93ed3eb74df908b19a38a55cd1e933`  
		Last Modified: Tue, 13 Oct 2020 07:08:46 GMT  
		Size: 68.7 MB (68748461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9396e96b868a452048c94dcb5a7186b3d8598527b47154f280ee1b28cf0dd231`  
		Last Modified: Tue, 13 Oct 2020 07:08:23 GMT  
		Size: 8.9 KB (8945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb9caafc4626f91d273ea4e68623cab234b8a0e7af0ef97e3b87f25ed23bec`  
		Last Modified: Tue, 13 Oct 2020 07:08:22 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9153637e645d8eeb572b0ec7ef47bf94fe3723a48f5be48434bea293586e1439`  
		Last Modified: Tue, 13 Oct 2020 07:08:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980bbb605244342a8f45561456202c2ffb09f9deb7ec43fa240e7a00d2690a5a`  
		Last Modified: Tue, 13 Oct 2020 07:08:22 GMT  
		Size: 4.3 KB (4255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d72adb35f673d3e4de74db50065f9a4ae2e41f25b13dd81ea147c22af9245f5`  
		Last Modified: Tue, 13 Oct 2020 07:08:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:0c474acf309f79e4d132b0cb1c47571cf6d088018d8b93ce34bb2fb4d35c75ec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110668665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cce592cdf7060da6e21abf6ab4224cc6c7d208fcf19133d684bf7a436bf6275c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:01:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 11:01:16 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 11:01:17 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 11:01:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 11:01:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 11:01:49 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 11:01:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:02:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 11:02:04 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 11:03:17 GMT
ENV PG_MAJOR=12
# Tue, 13 Oct 2020 11:03:18 GMT
ENV PG_VERSION=12.4-1.pgdg100+1
# Tue, 13 Oct 2020 11:03:49 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 11:03:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 11:03:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 11:03:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 13 Oct 2020 11:03:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 11:03:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 11:03:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 11:03:59 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 11:04:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 11:04:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 11:04:02 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 11:04:03 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 11:04:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b54dce2ac1eb5c484547daceb63d77b4ebf86f7adfd08524a95ce1aff995a0`  
		Last Modified: Tue, 13 Oct 2020 12:19:50 GMT  
		Size: 4.2 MB (4170140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35640a43c389c81984759b8bf006675c2a1e3022a8d2d264a668d146e4769dbd`  
		Last Modified: Tue, 13 Oct 2020 12:19:47 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954d8cf15b37983553c28d10814bd8446e8868be10ddf07020e44a34f42f42b0`  
		Last Modified: Tue, 13 Oct 2020 12:19:48 GMT  
		Size: 1.4 MB (1354215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cabadd29423fceb4b9404f0cd2f1acbbd9e1a5ae16cb2ede30fb5d61c03754d`  
		Last Modified: Tue, 13 Oct 2020 12:19:50 GMT  
		Size: 8.0 MB (7965226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1dd2db3831e8b25aa548ca0e46c9d5401d403008baebac964b6d92481f854b`  
		Last Modified: Tue, 13 Oct 2020 12:19:47 GMT  
		Size: 389.5 KB (389459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4df45b4efe24423097c32f0333b82820205f47b219e75a9ef9cb82de56f0b5`  
		Last Modified: Tue, 13 Oct 2020 12:19:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896ba7aabec2bed17223fe6f2f53f9d77908d0d1103da3be9285dd1916e12dd`  
		Last Modified: Tue, 13 Oct 2020 12:19:46 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26e2e8e8ad87f68a4a345684b17af3d7a76f4ec390ebbdb90f589920d525943`  
		Last Modified: Tue, 13 Oct 2020 12:20:39 GMT  
		Size: 70.9 MB (70921635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e724356110ef34e2e99353cccea4fae1804aadfd0e433a48e457b7ff1113bc`  
		Last Modified: Tue, 13 Oct 2020 12:20:17 GMT  
		Size: 8.9 KB (8937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b610ab4b13c5ca7bf664684633c12c4b067b8522d742ba8f5940adce951da15f`  
		Last Modified: Tue, 13 Oct 2020 12:20:17 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45adf2c83775382a26f0ec7a4009305f71095d93955e038fb9f95ac5ed0b4f0`  
		Last Modified: Tue, 13 Oct 2020 12:20:17 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b2e3a02f725c318650a91bb66e2486b40108699166ad5e4b10d40801dc2c59`  
		Last Modified: Tue, 13 Oct 2020 12:20:17 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7391f377fc9994a65c314837505a3472092fb8d7ec251136d39d0cccfa2360ff`  
		Last Modified: Tue, 13 Oct 2020 12:20:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; 386

```console
$ docker pull postgres@sha256:9ac69ab75fd982b72064780473e1cb169884ca14c8c77ce598de53b945dcf070
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115006760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be426aab762d4aa7b641cf5b0f478a53a9c268f0b4cd8108b6f26b7568746ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 16:41:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 16:41:02 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 16:41:02 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 16:41:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 16:41:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 16:41:23 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 16:41:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 16:41:30 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 16:42:13 GMT
ENV PG_MAJOR=12
# Tue, 13 Oct 2020 16:42:13 GMT
ENV PG_VERSION=12.4-1.pgdg100+1
# Tue, 13 Oct 2020 16:42:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 16:42:43 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 16:42:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 16:42:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 13 Oct 2020 16:42:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 16:42:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 16:42:47 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 16:42:48 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 16:42:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 16:42:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 16:42:50 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 16:42:50 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 16:42:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c749690104cd2d067ab453dc94a6cb768cf70e8de2c7b070e3ec6c77cbea76`  
		Last Modified: Tue, 13 Oct 2020 16:47:28 GMT  
		Size: 4.5 MB (4542310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e540fa0f9a8216d1625184511d7ae088dfb209a6bfbb7b01c9c28c386c29b`  
		Last Modified: Tue, 13 Oct 2020 16:47:25 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f01c54b9c4b48006dab4a6cb134885abb354aeded9eacda10b26e602331d0cb`  
		Last Modified: Tue, 13 Oct 2020 16:47:26 GMT  
		Size: 1.4 MB (1389505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabc4d4ec793f5e333d10d49bbf35728a1ddc5fa3b6e52c352e3d895ac7e082d`  
		Last Modified: Tue, 13 Oct 2020 16:47:31 GMT  
		Size: 8.0 MB (7964471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375c7950de1c2fb505ecd4b84309dceec40018957c961d9cea659485543b3d02`  
		Last Modified: Tue, 13 Oct 2020 16:47:24 GMT  
		Size: 398.2 KB (398247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bdf70f6f30cc05214496056e156b19a2a2e44644781822d902a04d7011b734`  
		Last Modified: Tue, 13 Oct 2020 16:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edb30201e63d9b68cdbed38ee43fd90089112ea5608240ebd879220b62db189`  
		Last Modified: Tue, 13 Oct 2020 16:47:23 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc7cd0204dc8d4f02611f6ad0dc2c271d9a7904f7e27e81bc9aa0499dcc6e03`  
		Last Modified: Tue, 13 Oct 2020 16:48:31 GMT  
		Size: 72.9 MB (72943427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3fbd48ae1591095cf875f883ca268303e1777a76005ec8304faa01b41a4a42`  
		Last Modified: Tue, 13 Oct 2020 16:48:01 GMT  
		Size: 8.9 KB (8945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a30ed5873c50735e954b355421837817aaae2b51d47825fa37ca3d2624dc2d`  
		Last Modified: Tue, 13 Oct 2020 16:48:01 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950c229f92e709ae7f42eeb93dff3f1d6364584f29bd23108e541560e12412a0`  
		Last Modified: Tue, 13 Oct 2020 16:48:01 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729c6798abe53bbda666565666eb61fbdb9111d0a482f6f6e959bb1d9b508439`  
		Last Modified: Tue, 13 Oct 2020 16:48:01 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9897ee9e375eb404515d9402df6a491e585e41fc734516f8c0cb0b3f423db816`  
		Last Modified: Tue, 13 Oct 2020 16:48:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; mips64le

```console
$ docker pull postgres@sha256:5adee7a313b1b20c911c7a2abc4f6aabc23d6bdc02ca160fd395b28d7e08bedf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (109968397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a14f1028a55a9a87cc95b2b76e4a4af1ac592e16f2ff509646c8034a126da65b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:13:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 13:13:38 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 13:13:38 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 13:13:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 13:14:23 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 13:14:24 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 13:14:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 13:14:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 13:14:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 14:06:51 GMT
ENV PG_MAJOR=12
# Tue, 13 Oct 2020 14:06:51 GMT
ENV PG_VERSION=12.4-1.pgdg100+1
# Tue, 13 Oct 2020 14:56:27 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 14:56:30 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 14:56:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 14:56:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 13 Oct 2020 14:56:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 14:56:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 14:56:35 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 14:56:36 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 14:56:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 14:56:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 14:56:38 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 14:56:38 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 14:56:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e607f4b85ab0160062c5b0997b24f9c552c3b0a99c818918df616f061bc1582`  
		Last Modified: Tue, 13 Oct 2020 14:57:06 GMT  
		Size: 4.2 MB (4182331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2e3c1d8252ef141fbeb05954df9c4cffe4be8a378178b0f7bc970a74a6c7a5`  
		Last Modified: Tue, 13 Oct 2020 14:57:02 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea3f4e38a84676f0d0f445a051330b19231188038d657dd3578c9ca400f1984`  
		Last Modified: Tue, 13 Oct 2020 14:57:03 GMT  
		Size: 1.3 MB (1307194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bc9170e37b7197108bb722eaee5a99c4b901d9be26a821a6b1d4db05f4362`  
		Last Modified: Tue, 13 Oct 2020 14:57:07 GMT  
		Size: 8.0 MB (7964635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab188a504bfa78fc88e311060cec8f95d3e3117d1419d605ac3ff070b82d000`  
		Last Modified: Tue, 13 Oct 2020 14:56:59 GMT  
		Size: 389.2 KB (389250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94c8867122219de48b09839756b0ffd313a762e792727c7390ae175987591ab`  
		Last Modified: Tue, 13 Oct 2020 14:56:59 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079c91791bcc494ca3ceef784e9686b641a2dfd712ce9279a1b3f406a9c2dce0`  
		Last Modified: Tue, 13 Oct 2020 14:56:59 GMT  
		Size: 3.1 KB (3060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea32488fc5f40ece2fbae0d7b23e13b4973f058e8d541775449a420bedb4b6a`  
		Last Modified: Tue, 13 Oct 2020 14:58:55 GMT  
		Size: 70.3 MB (70343835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec71ea362ca3ada7122902b3cbf72fa0bbd3ec812cedefa37e2e12f01de12c83`  
		Last Modified: Tue, 13 Oct 2020 14:58:04 GMT  
		Size: 8.9 KB (8947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf188bf74d39c9af1116cdcac376d148dafbfa4155346b92467b10bb0a16983`  
		Last Modified: Tue, 13 Oct 2020 14:58:04 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4346e4b2aec674e4bb96a16ffb7603b7eb10ba93452a31c24ff049a7a8597984`  
		Last Modified: Tue, 13 Oct 2020 14:58:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c00a95b6c9f97b792af27a401d2375f10d0940a39acac22925be28b41221e9`  
		Last Modified: Tue, 13 Oct 2020 14:58:04 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb236da9736f0863bd6de3ccc662f2da155842f9af72844a19d68efb06149151`  
		Last Modified: Tue, 13 Oct 2020 14:58:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; ppc64le

```console
$ docker pull postgres@sha256:7cb944169e8534a61e78956b3e2620a0471e45c2665f4a64360dace889e5d0bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121602041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad95087cdb8dbcd4e1e17f14b5cc9c19bb10f83afbfc574c2584dfac9dc67aab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:31:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:31:39 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:31:42 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:32:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:33:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:33:13 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:33:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:34:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:34:16 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:37:28 GMT
ENV PG_MAJOR=12
# Tue, 13 Oct 2020 12:37:35 GMT
ENV PG_VERSION=12.4-1.pgdg100+1
# Tue, 13 Oct 2020 12:39:23 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:39:40 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:39:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:39:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 13 Oct 2020 12:39:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:40:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:40:23 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:40:25 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:40:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:40:54 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:40:58 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:41:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561d545502ace2058d00663781db14dfa7756b6edb0acc8d79700400b867d9`  
		Last Modified: Tue, 13 Oct 2020 12:42:26 GMT  
		Size: 5.0 MB (4967255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ce5eebcabcdc9f2911ca87a8ab93cf539c873fa6cd96595dd928263e616b0`  
		Last Modified: Tue, 13 Oct 2020 12:42:22 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623858b6704dcb200beeee22ceb00bbeed4613a5b3d2df4ea7e457712e441d52`  
		Last Modified: Tue, 13 Oct 2020 12:42:22 GMT  
		Size: 1.3 MB (1337966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740971b5e3abf8f64361a1c8b2c4925b1c6f6a64ff7bd7482fa567278cd16ad6`  
		Last Modified: Tue, 13 Oct 2020 12:42:17 GMT  
		Size: 8.0 MB (7965414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8928d4fa7be49ec051fe27e367a44509f36af44275dabf2115d9dadadda84`  
		Last Modified: Tue, 13 Oct 2020 12:42:14 GMT  
		Size: 397.0 KB (397010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa177700b6800c9f06584f40ca975a9845416cfda21bc3e479c67addaf7aed1e`  
		Last Modified: Tue, 13 Oct 2020 12:42:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91522516c8e69fabb5c9cbbb1e69764d59bc27dfba6a6a86c1f1d334abdea069`  
		Last Modified: Tue, 13 Oct 2020 12:42:14 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60b348fe57697c088041086bd59712514981d6681eccbb535cacca238dbf78`  
		Last Modified: Tue, 13 Oct 2020 12:43:05 GMT  
		Size: 76.4 MB (76397849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a1e7a351491a5ad2ebda1f1e6a1fc87be7bcd68fa490c0d9128dd38c8d312e`  
		Last Modified: Tue, 13 Oct 2020 12:42:47 GMT  
		Size: 8.9 KB (8950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15ee3a75c153a5b35cb7d7767328a9c1e492a64658f8bac7b3637a7299bfe67`  
		Last Modified: Tue, 13 Oct 2020 12:42:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f79380fe437436e1c9187ada65dd5d122522021ba06cd433771f872f8a71ff`  
		Last Modified: Tue, 13 Oct 2020 12:42:47 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965739ac56c83da408da932b46648a78f60246159022292ae5f46e0af3b4d565`  
		Last Modified: Tue, 13 Oct 2020 12:42:47 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7e647d9e5f9eb45a795664ab5933ebda02d63389204d18e4a5cb4550dafa78`  
		Last Modified: Tue, 13 Oct 2020 12:42:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12` - linux; s390x

```console
$ docker pull postgres@sha256:6b94ebe6d5def9269a4ee72deef0d87b926d64875bec0b29073cba2e0ed998db
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80656898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c902bfd6ec8a637bb64a19c620000da83d5d8155954d479d9253788f94ddf4fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:29:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:29:42 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:29:43 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:29:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:30:00 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:30:01 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:30:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:30:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 05:39:52 GMT
ENV PG_MAJOR=12
# Tue, 13 Oct 2020 05:39:52 GMT
ENV PG_VERSION=12.4-1.pgdg100+1
# Tue, 13 Oct 2020 05:46:38 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 05:46:44 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 05:46:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 05:46:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 13 Oct 2020 05:46:46 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 05:46:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 05:46:47 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 05:46:48 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:46:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 05:46:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 05:46:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 05:46:49 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 05:46:50 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7246467ce71536a8e2ade5b913ba8c8c2c284426242907721099dceee57b3d`  
		Last Modified: Tue, 13 Oct 2020 05:47:38 GMT  
		Size: 4.1 MB (4059880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fbfd1313b673513f09c3f4ca8987bb77c156970039a431c5e677c2518b5ce7`  
		Last Modified: Tue, 13 Oct 2020 05:47:37 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316d02a9da51a3528085a50af6a3c3fc112a9892918038b44473e607269bce40`  
		Last Modified: Tue, 13 Oct 2020 05:47:37 GMT  
		Size: 1.4 MB (1406018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec69c124ec4c64206aeea60c42ea10de9b1af911bd0efc456c487758989c627`  
		Last Modified: Tue, 13 Oct 2020 05:47:36 GMT  
		Size: 8.0 MB (8019393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b1f52aea9588cf7dfe5864c787e643d0461967d4b63ce5186c896f2c7af72`  
		Last Modified: Tue, 13 Oct 2020 05:47:34 GMT  
		Size: 388.3 KB (388335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6429d50d17c8727d414f90680190cb9ff6d4d7e439a98bcb910575ed9cbf79`  
		Last Modified: Tue, 13 Oct 2020 05:47:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5cf466603f40623a27a57ca6f4c0148a2b16cfa2beaec1b72745cb3123df5d`  
		Last Modified: Tue, 13 Oct 2020 05:47:34 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daef3dbea86838f77ba593cf3d6a004eae21042ab58739df48854e8dc407e0a9`  
		Last Modified: Tue, 13 Oct 2020 05:48:00 GMT  
		Size: 41.1 MB (41057087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b62c18bd730321a9558bf2fab6842392bb00eb795f09d68b1cb0dc41bdc47b`  
		Last Modified: Tue, 13 Oct 2020 05:47:52 GMT  
		Size: 8.9 KB (8948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a752f92e733593d2396b5fb23dfa6d6d885e69aefae69c116b4fe72e21cc48e1`  
		Last Modified: Tue, 13 Oct 2020 05:47:52 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5c28989ab2da214733455e37f377b10dc6ef635413f48b46f9545f72d91280`  
		Last Modified: Tue, 13 Oct 2020 05:47:52 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9642f78da4c67692c9a346ce51bba8a68d78fe8e430c8b51f27198836a4285b`  
		Last Modified: Tue, 13 Oct 2020 05:47:52 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ccd49ee7844a375618860646e40daf0264273bdbcc2dcc88c21dfe0ce2666a`  
		Last Modified: Tue, 13 Oct 2020 05:47:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:12.5`

**does not exist** (yet?)

## `postgres:12.5-alpine`

**does not exist** (yet?)

## `postgres:12-alpine`

```console
$ docker pull postgres@sha256:e2759424387774dd8ddcbae936b885fa12fe6692b7875298e21e76f41375bd58
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
$ docker pull postgres@sha256:4c493832e4865189e3cab86281a1706a074ea6796b525a7f191b3f48546c25a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61358683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c9a6a10db626f333eca6009ea2e11ac23495b1e3bc3029aecac768a0722820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:55:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 07:55:14 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 07:55:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:01:06 GMT
ENV PG_MAJOR=12
# Thu, 22 Oct 2020 08:01:06 GMT
ENV PG_VERSION=12.4
# Thu, 22 Oct 2020 08:01:07 GMT
ENV PG_SHA256=bee93fbe2c32f59419cb162bcc0145c58da9a8644ee154a30b9a5ce47de606cc
# Thu, 22 Oct 2020 08:06:31 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:06:32 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:06:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:06:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:06:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:06:33 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:06:34 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:06:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:06:34 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:06:34 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:06:34 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f1d1b70e7fa650fd6229086120f763219adce9e33e8b20bdfbf8452ab69847`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4f01476d2b86761cdb0414c4a583b89af3b5d0b67022cfc0d378743307f7e3`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd0646b3208bb308c9f48cc278f01a0c7ef55a4eb3d7c1500dae51f34827a57`  
		Last Modified: Thu, 22 Oct 2020 08:22:16 GMT  
		Size: 58.5 MB (58547696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c638d1908b65ead9144d51423f0bd6afb8defef5e8bb2a17609789a80daadc`  
		Last Modified: Thu, 22 Oct 2020 08:22:07 GMT  
		Size: 8.2 KB (8211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f842fbbb0ac2b2f2cab3bce51147741243f3bc382f186dffd5dd4836f9a51351`  
		Last Modified: Thu, 22 Oct 2020 08:22:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e4714158403e3a4d71a5990a55c17c642f4559892d4bf882f69fb3dee8fd0b`  
		Last Modified: Thu, 22 Oct 2020 08:22:08 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149b4b732c76848655c8bb142e13d235673aad991eb4822aa6ee8f20e55e1658`  
		Last Modified: Thu, 22 Oct 2020 08:22:06 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:85231bd858960d66264daead20f142c14eb8c389047e2e2830796da9f3d945ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59609956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bafb3bffa13ad29372558ebe18efc4d4e0dfb0356dccf48f0f9de03a002344e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:55:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:55:00 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:55:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:00:06 GMT
ENV PG_MAJOR=12
# Thu, 22 Oct 2020 09:00:08 GMT
ENV PG_VERSION=12.4
# Thu, 22 Oct 2020 09:00:09 GMT
ENV PG_SHA256=bee93fbe2c32f59419cb162bcc0145c58da9a8644ee154a30b9a5ce47de606cc
# Thu, 22 Oct 2020 09:04:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:04:32 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:04:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:04:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:04:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:04:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:04:39 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:04:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:04:41 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:04:42 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:04:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54bc8a79538fa79db3e734327f2a73654bc80285dc55b7e4d8d206161ec79a9`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30574d1822b9e42c2a6da5e4a8f52ab65d88be941e497b4565382967ebd326f8`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe59d928d32198e7341b74ceab700801201249e92c73fb14694ebfcd0924856`  
		Last Modified: Thu, 22 Oct 2020 09:20:05 GMT  
		Size: 57.0 MB (56993791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adcf4c9c6f8c85fb7de4d863f6f8b5bd4dde0092c8dc59ce21b42f1253ff607`  
		Last Modified: Thu, 22 Oct 2020 09:19:46 GMT  
		Size: 8.2 KB (8212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cd50f81a28cce663c1ccbf4125ff45a19f9a5f56c1b681e3982dd94c7ba0e3`  
		Last Modified: Thu, 22 Oct 2020 09:19:46 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4aa2299c1fb69726a40f5ce499756891c0112a5d3029eb24715cc8f6b44acaf`  
		Last Modified: Thu, 22 Oct 2020 09:19:45 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb29f15c54ae03d7a61d10f1d2e29b4ca5e3b60a3be2014bee3e4df4186ecdfc`  
		Last Modified: Thu, 22 Oct 2020 09:19:46 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:c518aabf8e79df5f46b30d088d3f1d2db6aea7ea77aab6593226a624aa2ecd91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56743492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:535241b7ad8596da331d4e5380a88e1aae537ecb21894ead3fbf6aff816ece36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:56:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:56:03 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:56:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:00:10 GMT
ENV PG_MAJOR=12
# Thu, 22 Oct 2020 09:00:11 GMT
ENV PG_VERSION=12.4
# Thu, 22 Oct 2020 09:00:11 GMT
ENV PG_SHA256=bee93fbe2c32f59419cb162bcc0145c58da9a8644ee154a30b9a5ce47de606cc
# Thu, 22 Oct 2020 09:03:33 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:03:36 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:03:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:03:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:03:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:03:42 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:03:43 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:03:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:03:45 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:03:46 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:03:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7eedf40b1ca3ca0c12781ef9399626d49e7898eb4dc6bf3888a3add86c9ee2`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2cc4a27e16f2350721162545664e1c967b92e8a0ecffb90828c979f0bc3ac6`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db589e909616074bdbbcd301cdd6d065875bb040ba8180bff12ac6e610e4148e`  
		Last Modified: Thu, 22 Oct 2020 09:17:46 GMT  
		Size: 54.3 MB (54323561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0195b3c166d0f527d5d0d98199e851081e4497b2d27fefd03f6a0a67ca102aec`  
		Last Modified: Thu, 22 Oct 2020 09:17:31 GMT  
		Size: 8.2 KB (8214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da72bdd2bb91f0219fc0c570793307b0d7a0606b31a613c4c517b12413bc15d`  
		Last Modified: Thu, 22 Oct 2020 09:17:31 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4c3978c25e1d23cd988dc28dc19f5b8132a4aa074d380e3ef77d8b2d0cec5c`  
		Last Modified: Thu, 22 Oct 2020 09:17:31 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8918a7b79a3a9c7e02264c4bdefa2b20f9dbe0b5aa0e3e6b018c506de8cd20`  
		Last Modified: Thu, 22 Oct 2020 09:17:31 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:56b8bbbf198c216819b77650e924fa5448b9419ca2273d19871c33ade457adb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.9 MB (60933396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b810552dcd8fc417a6f0b7a2c1e7e593d16de1cc723388c43d188c5ad16814`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:21:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:21:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:21:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:26:00 GMT
ENV PG_MAJOR=12
# Thu, 22 Oct 2020 08:26:01 GMT
ENV PG_VERSION=12.4
# Thu, 22 Oct 2020 08:26:02 GMT
ENV PG_SHA256=bee93fbe2c32f59419cb162bcc0145c58da9a8644ee154a30b9a5ce47de606cc
# Thu, 22 Oct 2020 08:29:48 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:29:53 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:29:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:29:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:29:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:29:59 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:30:00 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:30:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:30:02 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:30:03 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:30:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b3b77440641e62ecc741cdb44f0f558d15c3f3b6d506be26f8c285f7a36ff`  
		Last Modified: Thu, 22 Oct 2020 08:44:00 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85615d5b5e22de086f665265885eae6f4cb41a63e5ed6910df6d0d03d0e90c5`  
		Last Modified: Thu, 22 Oct 2020 08:43:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f5db76c4f20ddb628d5db199061af2ecb11bd84776c87ac632bfd1093e7b7e`  
		Last Modified: Thu, 22 Oct 2020 08:44:37 GMT  
		Size: 58.2 MB (58212586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e055552abd2b888bcf94278309bc5650100822a40fa1d6e527d5e2fa93e290`  
		Last Modified: Thu, 22 Oct 2020 08:44:22 GMT  
		Size: 8.2 KB (8213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a12365626004f334f1ceed7768adc7260d1323b50876b6abd5cb02534c24a8`  
		Last Modified: Thu, 22 Oct 2020 08:44:22 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0728cdcb113ec594eb748ea8fc91ec925fd11b2c25ac269d3bb70c6e809b5236`  
		Last Modified: Thu, 22 Oct 2020 08:44:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f00d123c33dcd2c1be24d025c18ffa922b017fd6cda8e0e0e2c37eb1057f601`  
		Last Modified: Thu, 22 Oct 2020 08:44:23 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; 386

```console
$ docker pull postgres@sha256:39c5b27a0d8692f66cc68e7841a66ce1482deffa19a0e70a279f3d61d0c161a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64913049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99773c34e09d2d4af1ba0fbf41ab1b49f61c6b6ca29d66142972928efc69d212`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:38:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:38:39 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:38:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:47:38 GMT
ENV PG_MAJOR=12
# Thu, 22 Oct 2020 09:47:39 GMT
ENV PG_VERSION=12.4
# Thu, 22 Oct 2020 09:47:40 GMT
ENV PG_SHA256=bee93fbe2c32f59419cb162bcc0145c58da9a8644ee154a30b9a5ce47de606cc
# Thu, 22 Oct 2020 09:56:19 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:56:20 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:56:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:56:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:56:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:56:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:56:22 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:56:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:56:23 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:56:23 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:56:23 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596122efb908f979efd1794c09ae9c7a15ac0e4d53f2c181fd646d9f32565d9a`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeb7bd791d51cd161cadd22b53bd066e70998ebd55dd5ba92760d35f1ab9e8b`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fdeda581f2b91f542df0b373650dab6d068f2c2ee39070c9392e31daef2e7d`  
		Last Modified: Thu, 22 Oct 2020 10:21:35 GMT  
		Size: 62.1 MB (62107513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a13781a989b226cd89e636c655c6119600e6372c9c195b9c69e8b952b171d1`  
		Last Modified: Thu, 22 Oct 2020 10:21:13 GMT  
		Size: 8.2 KB (8212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df0b2352f7cb066a207afebc9212b042e03b3d9ab2431cdf1bd8aff592f0317`  
		Last Modified: Thu, 22 Oct 2020 10:21:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726b22a3ead84fd20920b6a321c86529ca58849db0b0caa0f2a6f37157b70a48`  
		Last Modified: Thu, 22 Oct 2020 10:21:13 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44db3a348d529a8f29211807fec770e8209e7a9304fadf3586cc9cf19830ff4`  
		Last Modified: Thu, 22 Oct 2020 10:21:12 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:4a3cd4a16aa80ea8a0f02318edc5058ffa0de0db0b7a0153b18d68cfafdd8cdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63722425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6af112c2ccea1344b9f6820f8ce5dd686c7171bb4ef2e09d426b15bace01f3e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 23:06:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 23:06:17 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 23:06:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 23:12:09 GMT
ENV PG_MAJOR=12
# Thu, 22 Oct 2020 23:12:22 GMT
ENV PG_VERSION=12.4
# Thu, 22 Oct 2020 23:12:29 GMT
ENV PG_SHA256=bee93fbe2c32f59419cb162bcc0145c58da9a8644ee154a30b9a5ce47de606cc
# Thu, 22 Oct 2020 23:16:48 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 23:17:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 23:17:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 23:17:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 23:17:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 23:17:58 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 23:18:02 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 23:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 23:18:16 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 23:18:27 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 23:18:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cba28bb2e7e5449306ade2eb73dd95379370b59f2eac45aa9f62aa4d376b1`  
		Last Modified: Thu, 22 Oct 2020 23:41:44 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b145001d871735701a01931a308a05fafba12a34115cac00163359d3ed8cf19`  
		Last Modified: Thu, 22 Oct 2020 23:41:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1954222b388327899a3e4080500fc3e458c0b214a43af9c14e557d24ed21cf`  
		Last Modified: Thu, 22 Oct 2020 23:42:32 GMT  
		Size: 60.9 MB (60904951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b197bcc9d55c63e088cfa3419fe53b20e6d6ffd330d5aff28edb66b84c7ec9`  
		Last Modified: Thu, 22 Oct 2020 23:42:15 GMT  
		Size: 8.2 KB (8209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efef4119ccb18442c58a7087ff076d02844975242fc0ab5bf5fba79bb029ac0`  
		Last Modified: Thu, 22 Oct 2020 23:42:15 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4d604caa3bdca2de8271e6750915bc7151093f61e73483f49bc35b9bcb239c`  
		Last Modified: Thu, 22 Oct 2020 23:42:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718aaec60ef32c403828675e40208c6b74efd5283c570a4ee7cc77f713237c66`  
		Last Modified: Thu, 22 Oct 2020 23:42:15 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:94976e9501f1856669f3a86d5a1dd6bdd258ae157eb024098239c16ff446a242
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63694331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00f55185828138bee7f29af67f47a550ba9629949638aba57997744f721b42c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:05:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:05:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:05:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:10:45 GMT
ENV PG_MAJOR=12
# Thu, 22 Oct 2020 09:10:45 GMT
ENV PG_VERSION=12.4
# Thu, 22 Oct 2020 09:10:46 GMT
ENV PG_SHA256=bee93fbe2c32f59419cb162bcc0145c58da9a8644ee154a30b9a5ce47de606cc
# Thu, 22 Oct 2020 09:14:42 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:14:51 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:14:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:14:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:14:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:14:55 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:14:55 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:14:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:14:57 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:14:57 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:14:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788b366e4c5d5f3b69b31ae06b2811fe54eb39bd4fd8b6107985f9982ab150a`  
		Last Modified: Thu, 22 Oct 2020 09:29:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eed686015d5efd53e62cc5b3f61833711a48184edf03c7d21f021b34f23095`  
		Last Modified: Thu, 22 Oct 2020 09:29:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528ac2f475893e6b29892702c935ba702d55bef7babd3bc95db7080479bf9cfc`  
		Last Modified: Thu, 22 Oct 2020 09:29:32 GMT  
		Size: 61.1 MB (61114242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e33996b03c7c8d98156abdba4f5f78a3091d86267f70c11347e1d7d6d5d66a9`  
		Last Modified: Thu, 22 Oct 2020 09:29:22 GMT  
		Size: 8.2 KB (8214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775c38d860bfac1a42cdeff32f1623e3e2b9c05af8dd445acb0ed4c5fe31d2d3`  
		Last Modified: Thu, 22 Oct 2020 09:29:22 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a26f26c1c1817fa6ad47a3e40769054ce9b83a6f783469954c6504c26df7768`  
		Last Modified: Thu, 22 Oct 2020 09:29:23 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7d16687b5bbc61bf345163638486be3252d5dbde8578f09f36003011afdfa`  
		Last Modified: Thu, 22 Oct 2020 09:29:22 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:13`

```console
$ docker pull postgres@sha256:8f7c3c9b61d82a4a021da5d9618faf056633e089302a726d619fa467c73609e4
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

### `postgres:13` - linux; amd64

```console
$ docker pull postgres@sha256:832e01fa055c55a9c9195db231cf3935a81b7b60c8cccd64e7b5395d1ee1948b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114727939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c96f8b6bc0d9f0277f118cf485a8c302e32cfe05e7d65f6e9a4c106679439d5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:31:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:31:49 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:31:49 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:31:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:32:06 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:32:07 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:32:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:32:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:32:13 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:32:14 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 12:32:14 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 12:32:34 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:32:35 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:32:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:32:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 12:32:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:32:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:32:37 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:32:37 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:32:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:32:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:32:38 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:32:39 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:32:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dc51fa2b560b7daf34aa4c2501941b4ce0d701c4ecf571777b13d79561f1bc`  
		Last Modified: Tue, 13 Oct 2020 12:37:32 GMT  
		Size: 4.2 MB (4178093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f213b6f96d81fa40e97b4eb61a159f716d77a4c70a25f376525385d7836bdee2`  
		Last Modified: Tue, 13 Oct 2020 12:37:31 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2780ac832fdea1b95491eaf082507289c13fc77e97de2716ee80e851cce0c79a`  
		Last Modified: Tue, 13 Oct 2020 12:37:31 GMT  
		Size: 1.4 MB (1419193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5cee1a3f123d23889bfdd0941b304d3906c90e136ec0e13f340b473096902f`  
		Last Modified: Tue, 13 Oct 2020 12:37:33 GMT  
		Size: 8.0 MB (7964517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95db3c06319e21f4c21eff545348f1755e5979d63c551a5b82bf9ff55ef30fa5`  
		Last Modified: Tue, 13 Oct 2020 12:37:30 GMT  
		Size: 391.1 KB (391050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475ca72764d52e2efe3b99160dbf36815c6be1ffda0790cc7e22354796185f08`  
		Last Modified: Tue, 13 Oct 2020 12:37:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d602872ecaeaf9c80cc4728578cc9a9b42d53b5f9351195a60f0be4455f99fd`  
		Last Modified: Tue, 13 Oct 2020 12:37:30 GMT  
		Size: 3.1 KB (3053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fca31f2e3d83c36758a751e320fd26cb77d6f17a5f07b73989d935ddbfd510`  
		Last Modified: Tue, 13 Oct 2020 12:37:46 GMT  
		Size: 73.7 MB (73663978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c442835e0871a8bcee1d389c603ff88190004b04ab5186d59836f2c3379e8`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 9.3 KB (9266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2305af339024dfd3d40697adb93e5ccb8decba5337e3eef1979ee4a2f151ca`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff852bb872a5b4dd86f2528157acb8c3ab2f59f5bce84a91e38990afb7e798`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bb0be115435b86fab9f9ac77ee9b01ca697d631038ff6e062ff203baf0a1fb`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 4.3 KB (4257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4738c099c4ad0480a6ea8a835aaf6777de42ec140984844cd53b9e05f8c44004`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13` - linux; arm variant v5

```console
$ docker pull postgres@sha256:38603a6ed6b60e32bd2c3358ae627f1d1abf2213c4b9a480895d6ca55c2b99a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.9 MB (108938865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd776c8231424dc528ba84f657cb51287071d6b6b792d2b328fe4e13f5c51a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:16:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 06:16:12 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 06:16:13 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 06:16:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 06:16:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 06:16:48 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 06:16:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:17:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 06:17:03 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 06:17:04 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 06:17:05 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 06:43:30 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 06:43:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 06:43:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 06:43:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 06:43:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 06:43:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 06:43:42 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 06:43:42 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:43:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 06:43:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:43:47 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 06:43:48 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 06:43:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220f749165a848f7f38bac836c52f4b835c99e7d95e05ee20dadaec192039226`  
		Last Modified: Tue, 13 Oct 2020 08:36:06 GMT  
		Size: 3.8 MB (3847907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99328c93a7de72d797aa8f54b8f5f65ac8dcfcb8adfcf619deb383521090b6a8`  
		Last Modified: Tue, 13 Oct 2020 08:36:05 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877588e4293d5c0bc10377dd6a2128f747be69e1e9176d0d8a2e6408917422ff`  
		Last Modified: Tue, 13 Oct 2020 08:36:05 GMT  
		Size: 1.4 MB (1378519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96f5e00aa670ea297c3d7b88aef48e3e83cecb4a2957ba6e1193fc4f3a0eba`  
		Last Modified: Tue, 13 Oct 2020 08:36:06 GMT  
		Size: 8.0 MB (7965207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e8a16e6b99574961ad43e457e425366fa1f111b3ce41c801ae3c66b5e68c86`  
		Last Modified: Tue, 13 Oct 2020 08:36:03 GMT  
		Size: 390.4 KB (390390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511e0945d4fb63b1f0366268b49f03e65681c8615d784c5ba2485563cf6d1f21`  
		Last Modified: Tue, 13 Oct 2020 08:36:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834364422035b3d7732f4346f19965cb41e38c4e33423185259f014337b1cfa0`  
		Last Modified: Tue, 13 Oct 2020 08:36:03 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf7b596aa05f83df06a644f9ce328ce279a1e0ba14b85696788de96ab737ddb`  
		Last Modified: Tue, 13 Oct 2020 08:36:25 GMT  
		Size: 70.5 MB (70501869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb22e708f1b3e5dff44453d0399222d13620e8be2f2c772c8d456c856f96da4`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 9.3 KB (9271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4403bcf196b9551826b50231481ba507bb6af5296da7e058aa8ca275bec41a2d`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa44359c6208940bde933378068055f585c04b80ccc76ec3d893142a68effd8d`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f819a8254858e6516d31a74081043ed355681e338f5849486a307a2aa19048e`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28de01a1ab0d2e4e95474888fc65ad4af854f91efa1f14f065382069ebc0917e`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13` - linux; arm variant v7

```console
$ docker pull postgres@sha256:9065c211f3d3b9f1f636403fcaa495416e6f3d1f194ffb957ab7ebf2119b4508
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104973664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28765e01da329697bcf5759441aad1e5e1ced29720adde286516666a1f31b0dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:03:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:03:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:03:10 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:03:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:03:51 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:03:52 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:04:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:04:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 05:04:10 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 05:04:11 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 05:29:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 05:29:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 05:29:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 05:29:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 05:29:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 05:29:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 05:29:16 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 05:29:17 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:29:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 05:29:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 05:29:21 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 05:29:21 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 05:29:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9abeb7fdbbade7b8abd012862e54cc393b34cd5ded22d30651c3d96f804017`  
		Last Modified: Tue, 13 Oct 2020 07:07:55 GMT  
		Size: 3.5 MB (3481628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c060aae45342f7e836211d989e2a8acbbc00aa77c9cedf463bc22d3931011b38`  
		Last Modified: Tue, 13 Oct 2020 07:07:54 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df78177be2b9c4f60b1d775bbe3774b00e3c1c567c4f122bbdff0d8c9be841a8`  
		Last Modified: Tue, 13 Oct 2020 07:07:54 GMT  
		Size: 1.4 MB (1370276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb71a60beb691d7f1f8351012f0a88049401c5ee2057e4a830758eee6c8dae4`  
		Last Modified: Tue, 13 Oct 2020 07:07:55 GMT  
		Size: 8.0 MB (7965243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3d3aab018a14d7c2ecdf71b6ba41d4a5521ba93a7a91a5ef2c466512f6165`  
		Last Modified: Tue, 13 Oct 2020 07:07:52 GMT  
		Size: 385.0 KB (385046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2443ca999a57081e3059a2ce066d226d974c0bfe22f8f887df06da48744d1b04`  
		Last Modified: Tue, 13 Oct 2020 07:07:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f35f400211e43d2986188ba441aee4ef58990df42a4f6215d473f4162cc97b5`  
		Last Modified: Tue, 13 Oct 2020 07:07:51 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7812530b8edbe3e8038a3f3ec17ae95fd1589ae6341af1725858e1d0b02394`  
		Last Modified: Tue, 13 Oct 2020 07:08:13 GMT  
		Size: 69.1 MB (69052639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f22889ebf9de2c6d34abee77286c2e5ff8184fd3b9e97d8a0ec4ff9303219fb`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 9.3 KB (9273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc99b88e591c236507bc93a29ac74921a6a9c6e09472065b67665870ed09f19`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a4c25625ec9a36c08c757ef59b112d266f6cef4d71a069746026f925ee9796`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eb3b82d2dfbb399ffeaff5992b19368614746e01205a39973031aa9bf667dc`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7031c8ae6bfe4c28598680fbfab04adb945f369033071a41102ccf52d070c6`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:0f96f9bd3099ebac30627729927a4be150465a669c0e79cf2fc94fda8c4f1248
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111040907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56731e2258858f1bf427e3050f388dc3e80d42b6077e433931c70fa32065a096`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:01:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 11:01:16 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 11:01:17 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 11:01:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 11:01:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 11:01:49 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 11:01:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:02:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 11:02:04 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 11:02:05 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 11:02:06 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 11:02:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 11:02:43 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 11:02:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 11:02:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 11:02:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 11:02:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 11:02:48 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 11:02:48 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 11:02:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 11:02:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 11:02:51 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 11:02:52 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 11:02:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b54dce2ac1eb5c484547daceb63d77b4ebf86f7adfd08524a95ce1aff995a0`  
		Last Modified: Tue, 13 Oct 2020 12:19:50 GMT  
		Size: 4.2 MB (4170140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35640a43c389c81984759b8bf006675c2a1e3022a8d2d264a668d146e4769dbd`  
		Last Modified: Tue, 13 Oct 2020 12:19:47 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954d8cf15b37983553c28d10814bd8446e8868be10ddf07020e44a34f42f42b0`  
		Last Modified: Tue, 13 Oct 2020 12:19:48 GMT  
		Size: 1.4 MB (1354215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cabadd29423fceb4b9404f0cd2f1acbbd9e1a5ae16cb2ede30fb5d61c03754d`  
		Last Modified: Tue, 13 Oct 2020 12:19:50 GMT  
		Size: 8.0 MB (7965226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1dd2db3831e8b25aa548ca0e46c9d5401d403008baebac964b6d92481f854b`  
		Last Modified: Tue, 13 Oct 2020 12:19:47 GMT  
		Size: 389.5 KB (389459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4df45b4efe24423097c32f0333b82820205f47b219e75a9ef9cb82de56f0b5`  
		Last Modified: Tue, 13 Oct 2020 12:19:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896ba7aabec2bed17223fe6f2f53f9d77908d0d1103da3be9285dd1916e12dd`  
		Last Modified: Tue, 13 Oct 2020 12:19:46 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598355fbe9f5b6cd68053bc6fe6357bb74394c1a74d2b8246e3fa01f4dddb68c`  
		Last Modified: Tue, 13 Oct 2020 12:20:05 GMT  
		Size: 71.3 MB (71293545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc69a8470043117cb274d54203477ac732c8cc100ce015512f6bcb3b24df6b9`  
		Last Modified: Tue, 13 Oct 2020 12:19:41 GMT  
		Size: 9.3 KB (9270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bea9860ee50eb0f0f3090fc98b246f3f1ff8797f292526285de1c6e77b573c`  
		Last Modified: Tue, 13 Oct 2020 12:19:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d44ba2b6c2bafc61dac4cb65a9a6da79a2eb11bce12324ae132d4cde3e631a8`  
		Last Modified: Tue, 13 Oct 2020 12:19:43 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1f22e595f6fdf38d7d04949e2ff149b9d62f547aa1cb0ec7c262af3bfe5f10`  
		Last Modified: Tue, 13 Oct 2020 12:19:41 GMT  
		Size: 4.3 KB (4257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f34ec236671db6a5b58d63a24446815ee2e0468f8826bba296f23dea12fd644`  
		Last Modified: Tue, 13 Oct 2020 12:19:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13` - linux; 386

```console
$ docker pull postgres@sha256:f018e9368b20e43b78fdb2913ac69058b0c1e97acee248d6b00765609237d6f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115393152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396efc10231f414e89419a0156bda225c11bb0060c11071bf85eebec57418980`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 16:41:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 16:41:02 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 16:41:02 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 16:41:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 16:41:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 16:41:23 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 16:41:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 16:41:30 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 16:41:30 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 16:41:30 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 16:41:56 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 16:41:57 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 16:41:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 16:41:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 16:41:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 16:41:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 16:41:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 16:41:59 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 16:42:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 16:42:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 16:42:01 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 16:42:01 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 16:42:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c749690104cd2d067ab453dc94a6cb768cf70e8de2c7b070e3ec6c77cbea76`  
		Last Modified: Tue, 13 Oct 2020 16:47:28 GMT  
		Size: 4.5 MB (4542310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e540fa0f9a8216d1625184511d7ae088dfb209a6bfbb7b01c9c28c386c29b`  
		Last Modified: Tue, 13 Oct 2020 16:47:25 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f01c54b9c4b48006dab4a6cb134885abb354aeded9eacda10b26e602331d0cb`  
		Last Modified: Tue, 13 Oct 2020 16:47:26 GMT  
		Size: 1.4 MB (1389505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabc4d4ec793f5e333d10d49bbf35728a1ddc5fa3b6e52c352e3d895ac7e082d`  
		Last Modified: Tue, 13 Oct 2020 16:47:31 GMT  
		Size: 8.0 MB (7964471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375c7950de1c2fb505ecd4b84309dceec40018957c961d9cea659485543b3d02`  
		Last Modified: Tue, 13 Oct 2020 16:47:24 GMT  
		Size: 398.2 KB (398247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bdf70f6f30cc05214496056e156b19a2a2e44644781822d902a04d7011b734`  
		Last Modified: Tue, 13 Oct 2020 16:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edb30201e63d9b68cdbed38ee43fd90089112ea5608240ebd879220b62db189`  
		Last Modified: Tue, 13 Oct 2020 16:47:23 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d0c377d25905e6dcc7b0de1ec1f2a925efa054feeaa7c4f346f5e646909a7`  
		Last Modified: Tue, 13 Oct 2020 16:47:55 GMT  
		Size: 73.3 MB (73329502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55cc6354a2dd5815e1a906ddf70063dc921507ad77e83ff37dae5169aa089eb`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 9.3 KB (9267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c77e86a23757931392202f1860011dca42b38ce451321f063b5173e3eb8d1f7`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0968e8f318a7dfc521a4a9dc8a9f35b5c096513aacaeda21888f91910aabf8`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af57a264872aebf23e30761bdd8f746d80cdde00ab2b6aca8f8becb55339782d`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dec4d85f466ca05a9c86992e601e395a740f8a0d8cf148f7bd57921a97818c`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13` - linux; mips64le

```console
$ docker pull postgres@sha256:6cdacd4e1e6463e0e88873d0293840c2db7fae74843994071b1e0995545574e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110310541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6c25d52c34151663ac0addf97fb0c57175829ccd2d35b3e80aea8d5728ffda6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:13:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 13:13:38 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 13:13:38 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 13:13:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 13:14:23 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 13:14:24 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 13:14:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 13:14:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 13:14:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 13:14:41 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 13:14:41 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 14:06:36 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 14:06:39 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 14:06:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 14:06:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 14:06:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 14:06:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 14:06:44 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 14:06:44 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 14:06:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 14:06:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 14:06:47 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 14:06:47 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 14:06:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e607f4b85ab0160062c5b0997b24f9c552c3b0a99c818918df616f061bc1582`  
		Last Modified: Tue, 13 Oct 2020 14:57:06 GMT  
		Size: 4.2 MB (4182331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2e3c1d8252ef141fbeb05954df9c4cffe4be8a378178b0f7bc970a74a6c7a5`  
		Last Modified: Tue, 13 Oct 2020 14:57:02 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea3f4e38a84676f0d0f445a051330b19231188038d657dd3578c9ca400f1984`  
		Last Modified: Tue, 13 Oct 2020 14:57:03 GMT  
		Size: 1.3 MB (1307194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bc9170e37b7197108bb722eaee5a99c4b901d9be26a821a6b1d4db05f4362`  
		Last Modified: Tue, 13 Oct 2020 14:57:07 GMT  
		Size: 8.0 MB (7964635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab188a504bfa78fc88e311060cec8f95d3e3117d1419d605ac3ff070b82d000`  
		Last Modified: Tue, 13 Oct 2020 14:56:59 GMT  
		Size: 389.2 KB (389250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94c8867122219de48b09839756b0ffd313a762e792727c7390ae175987591ab`  
		Last Modified: Tue, 13 Oct 2020 14:56:59 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079c91791bcc494ca3ceef784e9686b641a2dfd712ce9279a1b3f406a9c2dce0`  
		Last Modified: Tue, 13 Oct 2020 14:56:59 GMT  
		Size: 3.1 KB (3060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ed439ff0db80133ad5c64fd6f680da2629710df67c477195efe628627f8aa9`  
		Last Modified: Tue, 13 Oct 2020 14:57:49 GMT  
		Size: 70.7 MB (70685659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ef9de52f6e2ba62c847999fa0535d0640c61757dbce18666ef659edd3a715c`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 9.3 KB (9271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306e8acbffe7d13f0aff7b96ee72fb777ff29690469d9a9c6abcdb37686be56`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102f301ca71ccd15c8150f9420fe86cb7f59885a1f4d0742fc76d7cff131dc4`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563574ec7e322fff2134f1556e556d32d17984dd3a35fb760389b3fd08551a7`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e039d4d6237abc30a0d5f84382970f19bd8bd887db7069953d0c3a122ce3ad`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13` - linux; ppc64le

```console
$ docker pull postgres@sha256:cb47cd3347f142ab699462939df23ed7ab245a76ecca75c6c7143e1707c5694c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122023914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8032178de335da47dffe309bcfdb072cbed6334b8d2a45717a1b891963c3d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:31:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:31:39 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:31:42 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:32:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:33:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:33:13 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:33:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:34:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:34:16 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:34:20 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 12:34:24 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 12:35:57 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:36:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:36:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:36:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 12:36:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:36:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:36:43 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:36:44 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:36:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:37:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:37:03 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:37:07 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:37:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561d545502ace2058d00663781db14dfa7756b6edb0acc8d79700400b867d9`  
		Last Modified: Tue, 13 Oct 2020 12:42:26 GMT  
		Size: 5.0 MB (4967255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ce5eebcabcdc9f2911ca87a8ab93cf539c873fa6cd96595dd928263e616b0`  
		Last Modified: Tue, 13 Oct 2020 12:42:22 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623858b6704dcb200beeee22ceb00bbeed4613a5b3d2df4ea7e457712e441d52`  
		Last Modified: Tue, 13 Oct 2020 12:42:22 GMT  
		Size: 1.3 MB (1337966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740971b5e3abf8f64361a1c8b2c4925b1c6f6a64ff7bd7482fa567278cd16ad6`  
		Last Modified: Tue, 13 Oct 2020 12:42:17 GMT  
		Size: 8.0 MB (7965414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8928d4fa7be49ec051fe27e367a44509f36af44275dabf2115d9dadadda84`  
		Last Modified: Tue, 13 Oct 2020 12:42:14 GMT  
		Size: 397.0 KB (397010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa177700b6800c9f06584f40ca975a9845416cfda21bc3e479c67addaf7aed1e`  
		Last Modified: Tue, 13 Oct 2020 12:42:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91522516c8e69fabb5c9cbbb1e69764d59bc27dfba6a6a86c1f1d334abdea069`  
		Last Modified: Tue, 13 Oct 2020 12:42:14 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420d0a7efbf19ebce8f0088536a373b3205d7466526a64b3dae9f5423362edc0`  
		Last Modified: Tue, 13 Oct 2020 12:42:29 GMT  
		Size: 76.8 MB (76819402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32c8c22f6099516385dade75212072689a00ecaa4e2034386050b6b785c8529`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 9.3 KB (9268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92629bd5781650a7387e7af4a085d350ab77b488099d6e82ce955f2f03ffe57d`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7347194451e408bb9299f91edc3f6c9f3dce6779ed0ccf606fdb9f162b038165`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9193f231104f9dfe1bdb76f320002ba8f6730d35c8f8fa475ae27ad533682c6`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30870777ec22e86f3dba3808deb5da9b9a5427e1c804b15d21140d9c9e51424e`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13` - linux; s390x

```console
$ docker pull postgres@sha256:0aab83a6545cdd6b3814844c7b27a15e7ebc25fdb3d1d24610e73c21cc7db077
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.0 MB (113041886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50ac0b622ec547412072ab8b679c2d557f7172284518c9caf272ddb43aec4ca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:29:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:29:42 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:29:43 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:29:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:30:00 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:30:01 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:30:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:30:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 05:30:07 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 05:30:08 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 05:39:30 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 05:39:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 05:39:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 05:39:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 05:39:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 05:39:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 05:39:36 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 05:39:36 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:39:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 05:39:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 05:39:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 05:39:38 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 05:39:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7246467ce71536a8e2ade5b913ba8c8c2c284426242907721099dceee57b3d`  
		Last Modified: Tue, 13 Oct 2020 05:47:38 GMT  
		Size: 4.1 MB (4059880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fbfd1313b673513f09c3f4ca8987bb77c156970039a431c5e677c2518b5ce7`  
		Last Modified: Tue, 13 Oct 2020 05:47:37 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316d02a9da51a3528085a50af6a3c3fc112a9892918038b44473e607269bce40`  
		Last Modified: Tue, 13 Oct 2020 05:47:37 GMT  
		Size: 1.4 MB (1406018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec69c124ec4c64206aeea60c42ea10de9b1af911bd0efc456c487758989c627`  
		Last Modified: Tue, 13 Oct 2020 05:47:36 GMT  
		Size: 8.0 MB (8019393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b1f52aea9588cf7dfe5864c787e643d0461967d4b63ce5186c896f2c7af72`  
		Last Modified: Tue, 13 Oct 2020 05:47:34 GMT  
		Size: 388.3 KB (388335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6429d50d17c8727d414f90680190cb9ff6d4d7e439a98bcb910575ed9cbf79`  
		Last Modified: Tue, 13 Oct 2020 05:47:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5cf466603f40623a27a57ca6f4c0148a2b16cfa2beaec1b72745cb3123df5d`  
		Last Modified: Tue, 13 Oct 2020 05:47:34 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511d1c3258fd3b50e59f2508c15a8012230255ffaadb4a60b3e627e45a528d2c`  
		Last Modified: Tue, 13 Oct 2020 05:47:44 GMT  
		Size: 73.4 MB (73441752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320a06bf97139418261449c854dd4c2c5f3c62cc46a7ec5b79db8df49ef2d0`  
		Last Modified: Tue, 13 Oct 2020 05:47:32 GMT  
		Size: 9.3 KB (9271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4964cb4e537ebb6eb9840daa00c600a9fb570b5eb8a25db62f692d995d7443c`  
		Last Modified: Tue, 13 Oct 2020 05:47:33 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7a1074d81612d7507a6fe22514c36a9e5c1d65acd408b92640e10767898c85`  
		Last Modified: Tue, 13 Oct 2020 05:47:32 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305ce2b8a378c07a61cbc72936f4f9f922e7bc65147995fb54d39590fa774d8e`  
		Last Modified: Tue, 13 Oct 2020 05:47:32 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d384c65ea5d63596390498b0b7ea2023e387bb9d771fbd297a40e5180fb480d5`  
		Last Modified: Tue, 13 Oct 2020 05:47:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:13.1`

**does not exist** (yet?)

## `postgres:13.1-alpine`

**does not exist** (yet?)

## `postgres:13-alpine`

```console
$ docker pull postgres@sha256:d26ddee3648a324a9747b3257236322141920d5f9a82ca703def6bff1cca7067
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

### `postgres:13-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:28305dfe369277a8eaf90486c19c5d892653b914eac13b3b8b88521058b2e903
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62014089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700e581c202ecba5ce3ffe5908a9776163a4949d289caa8319245ca9cfc6b832`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:55:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 07:55:14 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 07:55:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 07:55:15 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 07:55:15 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 07:55:15 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 08:00:51 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:00:52 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:00:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:00:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:00:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:00:54 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:00:54 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:00:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:00:54 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:00:54 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:00:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f1d1b70e7fa650fd6229086120f763219adce9e33e8b20bdfbf8452ab69847`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4f01476d2b86761cdb0414c4a583b89af3b5d0b67022cfc0d378743307f7e3`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16419214bc023bd78d6b9098a87072ef74c349622f7320d0c84b6f326fd8b3e6`  
		Last Modified: Thu, 22 Oct 2020 08:22:00 GMT  
		Size: 59.2 MB (59202778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4886fc567835ca23c2e896a575abd09db4d3db62f1df7221bf053f624a8931cd`  
		Last Modified: Thu, 22 Oct 2020 08:21:51 GMT  
		Size: 8.5 KB (8534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9026d4fbeafa49378c5217a9f58a95633d2fcc3ea787a432d94fdbc3071e8a2c`  
		Last Modified: Thu, 22 Oct 2020 08:21:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001c336294ebcf88942d1d10c0387a319b47e9a799cea995ba87eac8c6c7760d`  
		Last Modified: Thu, 22 Oct 2020 08:21:51 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc6d154e9fb24a05c2186f1caa1d911119a82c4b2510186de584efc34dd40b`  
		Last Modified: Thu, 22 Oct 2020 08:21:51 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:9aa3390ad0b1f9eddc310269664accd38f81fa23cc91ae93d8cde6f06fb6bdf6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60195390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d24267bdc9a6b2208fc593a7eec2b1f769c57ab6946d77ecbe82b555ce85a279`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:55:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:55:00 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:55:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:55:03 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 08:55:03 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 08:55:04 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 08:59:31 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:59:35 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:59:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:59:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:59:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:59:42 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:59:43 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:59:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:59:46 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:59:48 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:59:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54bc8a79538fa79db3e734327f2a73654bc80285dc55b7e4d8d206161ec79a9`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30574d1822b9e42c2a6da5e4a8f52ab65d88be941e497b4565382967ebd326f8`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1745f68cca415c7401eeaea782a52b2a9dd04a3da1e4f3ce0a4c41a4c6fa74f7`  
		Last Modified: Thu, 22 Oct 2020 09:19:36 GMT  
		Size: 57.6 MB (57578893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137f32c2f9bfab96f1336bd6d701e161f61294427613777bf68e9675475ccb20`  
		Last Modified: Thu, 22 Oct 2020 09:19:17 GMT  
		Size: 8.5 KB (8542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2099ca9f5b36ba12428c29dcff2f9ff5e1561067c9c539f3cf2f10403b73918d`  
		Last Modified: Thu, 22 Oct 2020 09:19:17 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1490f1ec1eeec24777384af72b9b5b4c3952bb6d590e30463397dd923151358b`  
		Last Modified: Thu, 22 Oct 2020 09:19:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12193f12354e79945caf7850ac8fcd582ab67847fcca23df0046eb75dcfb8`  
		Last Modified: Thu, 22 Oct 2020 09:19:17 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:36ed8010aa7cb12ba66b1e4db0b8085fe08a61fc4f20b14c9dc5cf48f49fe391
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57304236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d095d11ad7acb1affe24fc9e4de91bbd54cb60004fd5315f80de26809f170dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:56:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:56:03 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:56:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:56:06 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 08:56:08 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 08:56:10 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 08:59:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:59:43 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:59:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:59:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:59:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:59:51 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:59:52 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:59:53 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:59:54 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:59:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7eedf40b1ca3ca0c12781ef9399626d49e7898eb4dc6bf3888a3add86c9ee2`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2cc4a27e16f2350721162545664e1c967b92e8a0ecffb90828c979f0bc3ac6`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9e1fc344fdc1be9247f34eb1533fd8a223cbab00b5bf4aa7459424df790ea4`  
		Last Modified: Thu, 22 Oct 2020 09:17:22 GMT  
		Size: 54.9 MB (54883977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65080db56689834b20ad68241bde5ccfa334bf0c2f80db744db6186238d2c89d`  
		Last Modified: Thu, 22 Oct 2020 09:17:06 GMT  
		Size: 8.5 KB (8540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3d3a7196b2ada5397485bfe080afd7d743d37f68d526f285b6a57887087e78`  
		Last Modified: Thu, 22 Oct 2020 09:17:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba4958fec54abe667c1f75d7c7f24dd84d87711ae546e91a16344740aeab57b`  
		Last Modified: Thu, 22 Oct 2020 09:17:06 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0fabe1fbf3b332a3379ec29ec509a3f837c46f5aac0601b8ee836c80fb9029`  
		Last Modified: Thu, 22 Oct 2020 09:17:06 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:b6399aef923e0529a4f2a5874e8860d29cef3726ab7079883f3368aaa2a9f29c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61557698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b98a8adac19738d6d88e76787142368522635722706e167bdfb7e3756f615b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:21:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:21:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:21:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:21:52 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 08:21:52 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 08:21:53 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 08:25:12 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:25:19 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:25:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:25:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:25:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:25:32 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:25:33 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:25:35 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:25:37 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:25:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b3b77440641e62ecc741cdb44f0f558d15c3f3b6d506be26f8c285f7a36ff`  
		Last Modified: Thu, 22 Oct 2020 08:44:00 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85615d5b5e22de086f665265885eae6f4cb41a63e5ed6910df6d0d03d0e90c5`  
		Last Modified: Thu, 22 Oct 2020 08:43:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3399ca8ba311608fce7edea2b4b7c56e3a15651820560e526d7e892a45d9a694`  
		Last Modified: Thu, 22 Oct 2020 08:44:11 GMT  
		Size: 58.8 MB (58836563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37765dcba1abe0ee860486e0de0391cb6816ed272cea1886bc75908efac1cf77`  
		Last Modified: Thu, 22 Oct 2020 08:43:58 GMT  
		Size: 8.5 KB (8539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2093493e16e25a2e3387389fa691fab3e9a5815dd691af0c7b6f055110d738f`  
		Last Modified: Thu, 22 Oct 2020 08:43:58 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e2815f4ac9a0a90fcaf51162bacb8adcd984d8958d89c016d82c79d5291fb3`  
		Last Modified: Thu, 22 Oct 2020 08:43:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df26ccc1cae9303c03384992f898557df12827808b6800a3ac24718d80dbc9`  
		Last Modified: Thu, 22 Oct 2020 08:43:58 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; 386

```console
$ docker pull postgres@sha256:1dfcbfea3e85ad81b7baef84a68c8d8f8676a6b400d1ff0790929bfe1bd6d9df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65604483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201098a3f6fa14cb91820bdfbfd34469df38d7dafe93450159291da47be86f3d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:38:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:38:39 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:38:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:38:40 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 09:38:40 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 09:38:41 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 09:47:21 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:47:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:47:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:47:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:47:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:47:25 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:47:25 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:47:25 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:47:26 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:47:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596122efb908f979efd1794c09ae9c7a15ac0e4d53f2c181fd646d9f32565d9a`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeb7bd791d51cd161cadd22b53bd066e70998ebd55dd5ba92760d35f1ab9e8b`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56896d944158831966b1797385c95616538974e5cd57e33ee6bd394de35b5b8e`  
		Last Modified: Thu, 22 Oct 2020 10:21:05 GMT  
		Size: 62.8 MB (62798615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6950449e6370c7a2e01599167c24c286b62f137d8ba017ccfd7650de7b5ba81a`  
		Last Modified: Thu, 22 Oct 2020 10:20:49 GMT  
		Size: 8.5 KB (8540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f993f62e6dccbb32c783ca06e482ddeba6cb723691026cde0c4fd16a81680558`  
		Last Modified: Thu, 22 Oct 2020 10:20:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f2b5e39d9584dfb53e36f59b5c9d94c757d9307ee3cdce7ce4ff0a6b43414`  
		Last Modified: Thu, 22 Oct 2020 10:20:49 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51377623be83e9b7af021a2b97dde5a2e68d0a43c1ad5405d32ad212a1c717de`  
		Last Modified: Thu, 22 Oct 2020 10:20:50 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:10d3658d045ccb6cf6e82b372cc302bdefbadd38713b567e2980d74217492efa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64406140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897a372ceb92ff324466d266bad1e31208f1441ea3284ec9e803f0f6f1bb6649`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 23:06:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 23:06:17 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 23:06:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 23:06:26 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 23:06:29 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 23:06:32 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 23:10:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 23:10:52 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 23:11:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 23:11:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 23:11:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 23:11:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 23:11:25 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 23:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 23:11:33 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 23:11:40 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 23:11:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cba28bb2e7e5449306ade2eb73dd95379370b59f2eac45aa9f62aa4d376b1`  
		Last Modified: Thu, 22 Oct 2020 23:41:44 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b145001d871735701a01931a308a05fafba12a34115cac00163359d3ed8cf19`  
		Last Modified: Thu, 22 Oct 2020 23:41:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d44cb7df0f4a70bbb8da1179c1ea586f8471e5720d0de26a1320d99ecfee94`  
		Last Modified: Thu, 22 Oct 2020 23:41:56 GMT  
		Size: 61.6 MB (61588341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0b9784976dc58199c67ea1dfa2df4d68566c102d7d1c6070322634c7ebfb6`  
		Last Modified: Thu, 22 Oct 2020 23:41:40 GMT  
		Size: 8.5 KB (8539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a35e1a562102237feab8796d8e9c6f6866dfadf1efc57d1b329b2d221d66d88`  
		Last Modified: Thu, 22 Oct 2020 23:41:41 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4facb5bf19a8bb8f97f75e520566074ccae805f4b863d6e48d699c4b204908b`  
		Last Modified: Thu, 22 Oct 2020 23:41:40 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8082c85c7c0de55885ba799e76111f5e1b288bef480873b2cecd123bd1af223`  
		Last Modified: Thu, 22 Oct 2020 23:41:41 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:e5a1e46e00aac62a7a70a4ee5811850b00267b3eabbe0c36bfb173014b996930
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64479911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeac1e50499ae7b21de2a4952e8bd9bc474c80b6e400748dcc3390fab7f07afa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:05:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:05:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:05:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:05:51 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 09:05:51 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 09:05:52 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 09:10:07 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:10:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:10:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:10:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:10:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:10:19 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:10:20 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:10:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:10:21 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:10:21 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:10:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788b366e4c5d5f3b69b31ae06b2811fe54eb39bd4fd8b6107985f9982ab150a`  
		Last Modified: Thu, 22 Oct 2020 09:29:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eed686015d5efd53e62cc5b3f61833711a48184edf03c7d21f021b34f23095`  
		Last Modified: Thu, 22 Oct 2020 09:29:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b5c49866375be63b5c0df20d45eff9b155100b10e2dad36b6369fa8dcb1e2d`  
		Last Modified: Thu, 22 Oct 2020 09:29:13 GMT  
		Size: 61.9 MB (61899505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b283091e8db48015a3a673e2074af8a40665adc59da43ae21251bc54e3fcd8`  
		Last Modified: Thu, 22 Oct 2020 09:29:04 GMT  
		Size: 8.5 KB (8535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb452e6ac31ed779bdb65f15850af5b72bc90c8a4031dd945a1c2a3adb16a75`  
		Last Modified: Thu, 22 Oct 2020 09:29:04 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc54b509173838bf179855e6124b92bc8f5d7f55809b0956165e22290c5d5c3`  
		Last Modified: Thu, 22 Oct 2020 09:29:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab84a2f6ff3bdde6b5575c71c358f3642d9fa6ad4b91ccdcce2fe3d43dc2bd6`  
		Last Modified: Thu, 22 Oct 2020 09:29:04 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9`

```console
$ docker pull postgres@sha256:56b556d681143501e02f794d149213e7b04e0fde814689e8efeaba64cf5b86be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:9` - linux; amd64

```console
$ docker pull postgres@sha256:7e2f12cb4aac2ac43ece76a6f49a12c9600b1fd70bd8471a67aeef070c2de7c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73508700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb00980cabc0d97647ae88849823eca58fe70505addbefdf7073127f2554ce34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:33:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:33:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:33:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:33:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:34:01 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:34:02 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:34:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:34:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:34:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:35:57 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 12:35:57 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 12:36:13 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:36:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:36:15 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:36:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 12:36:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:36:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:36:18 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:36:18 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:36:20 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:36:20 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:36:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0526c44df6ea5bd7668eab6d9c37d43aef6474cb4f5b6d2539e82404a3827041`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 4.5 MB (4502050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2466ee00e96ac149c287cdd533cecad2907d0aea2f2fe5ffc7a706ab313aaac`  
		Last Modified: Tue, 13 Oct 2020 12:38:27 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c605d60192c83f6a890b4f0cfaf8d80cf2a7a5c0c8df01451a106305748bf2`  
		Last Modified: Tue, 13 Oct 2020 12:38:28 GMT  
		Size: 1.4 MB (1412112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b14ab418421f0d1e9fb147720201f216050e2ad983640a446e75249e84e9bc`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 6.2 MB (6182797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f557fff31511f1f9475342998e8b195c0942480fb4901dab214f015d2224c`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 384.9 KB (384916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bba27806f46c2448fe4d5a0b248fd9178ced6163b8e2154e4b06a86c9a08b4`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e1555090548b1ab5739971b4eea16b502cc1e625f3a0b827463c4ae69bcc61`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228bfc35d59ec7fb6c7674ce61b84920448a676e97f868c2ef8190190af14d24`  
		Last Modified: Tue, 13 Oct 2020 12:39:16 GMT  
		Size: 38.5 MB (38484982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6d4aade3a7a4e37446351fb71d60240d112a86381462748f324dce24ac198`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 7.8 KB (7815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38f3152b7fdf51d67c1f9e1790a492c7db0a481733f64512417edb9753db19`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98e6187ea21bcec2504768d21903f612670c424ebf74cb3a5c4c47521de5de`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7ef009703566e3b88a5efa2d86e07bb1625e73962d31806810c1ed6aee6896`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 4.3 KB (4271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbb62021d40d5ab03a07921d007c562b870a110b52fffea952a8b278ea85457`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; arm variant v5

```console
$ docker pull postgres@sha256:ca7856a8accf79f12b00ac75d43ac2370f94bb915376c326b36b298776d22bae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70430486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0b6923e37593fae3669f514ff41c7acd2072dc9e8453088c77777811de62c79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:57:28 GMT
ADD file:ef761876435f34dd5e73f6fb89eda5cee26b26d9183a37dc5588c6eb5fd4ba69 in / 
# Tue, 13 Oct 2020 01:57:29 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 07:10:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 07:10:23 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 07:10:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 07:11:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 07:11:15 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 07:11:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:11:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 07:11:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 07:55:24 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 07:55:25 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 08:15:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 08:15:45 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 08:15:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 08:15:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 08:15:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 08:15:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 08:15:53 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 08:15:54 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:15:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 08:15:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:15:58 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 08:15:59 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 08:16:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e6fa5ab8c49c07aa49f655f00f7742fc2640bec642d3e0b440a9d67c37d1383e`  
		Last Modified: Tue, 13 Oct 2020 02:05:36 GMT  
		Size: 21.2 MB (21194476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4a7d58f9de066b4eb914552800ca9b9c3bdbd3a49d22592a568fd65353b60e`  
		Last Modified: Tue, 13 Oct 2020 08:37:11 GMT  
		Size: 4.2 MB (4238677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d9d67c7f2447a0677783317716fd66e891874c5dec4c300963bdaedef3db73`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8dfd96a4ee2041e6cf18fbfb05eaaf56b746f396297762c746643158da072a`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.4 MB (1371374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55137faf878bb43f0e314a0845bb679c3834709fb30668a8a966d3ea7d6324c6`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 6.2 MB (6185655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c626e10cc735d164b870d78d396556ebae2e833924a9782fc8880333228fea`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 385.1 KB (385110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5193a2411b31608c76d06bf9efa210a7cf0d1b51953e39d3cdc458342b259a86`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71923a948044364e5093b7b7e4e2667ee46f8e6fc34ff01d72050cd7aefbe702`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 5.3 KB (5350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4c3b81731670fd755cfdb0288eba11d45531b0f20ca8403f749cfecb7b5ca`  
		Last Modified: Tue, 13 Oct 2020 08:38:06 GMT  
		Size: 37.0 MB (37035346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8090714820c2155ccec56ed8b32cc8c3f629df37306bbafb73d090290515b0af`  
		Last Modified: Tue, 13 Oct 2020 08:37:49 GMT  
		Size: 7.8 KB (7820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869ebf10e05a7071d6297a796991331fe77699ddd6c06be50a95c7915120d49e`  
		Last Modified: Tue, 13 Oct 2020 08:37:48 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6407a17dd66fe517830ebd77c7711abe5ad5e370aadad7bcbbf9b7f3a940f3`  
		Last Modified: Tue, 13 Oct 2020 08:37:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9f5ca54f96ae786eb52e72557dcf9a6099e3eb7ee9304e8d7d10a6b110a124`  
		Last Modified: Tue, 13 Oct 2020 08:37:48 GMT  
		Size: 4.3 KB (4273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289ab3f2ecdbf9d195a9265f32e931fa915c9c3f16234315b35d83d2c2c40008`  
		Last Modified: Tue, 13 Oct 2020 08:37:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; arm variant v7

```console
$ docker pull postgres@sha256:31b3cd029967319dc19246604401d0d6b7799479c1e93293be0a653d15a94154
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67116658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb26ab48758ca5206f2fc7b879a00a884505072b6491ef4c0693156139683c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:04:30 GMT
ADD file:d204a257433edcd6f9ddd2c769b9e187c408eb4972203a5daab60214b5b576bc in / 
# Tue, 13 Oct 2020 01:04:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:54:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:54:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:54:44 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:55:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:55:24 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:55:25 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:55:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:55:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:55:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 06:32:53 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 06:32:54 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 06:50:04 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 06:50:08 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 06:50:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 06:50:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 06:50:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 06:50:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 06:50:14 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 06:50:14 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:50:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 06:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:50:18 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 06:50:19 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 06:50:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cc11be355171b10881b3ed16be16ceb2d7787cd459c6489d83bac55ee5824b35`  
		Last Modified: Tue, 13 Oct 2020 01:12:46 GMT  
		Size: 19.3 MB (19304540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8b70af887483c86f21ffd35a2a331fbab0ae0804a4929517360da6207fe6c3`  
		Last Modified: Tue, 13 Oct 2020 07:09:01 GMT  
		Size: 3.9 MB (3874946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09233e1347145a65db2aae548df648e91df34bde91664ac04509ff8ba2d77447`  
		Last Modified: Tue, 13 Oct 2020 07:08:59 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a09c7350562aee4559820b5fa1133618b8c02e7848e0c14635fb483b5a10fb`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 1.4 MB (1363819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9deba20fbd610072e97a51ac7766bcfdac37c6110ee53cdf296e7435868b5e7`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 6.2 MB (6185495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a750e8984fdec76cc5aa76a7979cd403c03d5b18efe690ebda5984356654554`  
		Last Modified: Tue, 13 Oct 2020 07:08:58 GMT  
		Size: 379.2 KB (379196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bd92fced2d524fc75c7429ca11a3f1c30587399ca0a571b4f623a3db6c15c2`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059b3634dc4169b9d362c9bf8d29e4c9af7a58bd40538452efeb506841942fb4`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee03b7c7b17e1992d1b43f10c016e8fc7369f82c5d3b8d9ab28526dda9e624d`  
		Last Modified: Tue, 13 Oct 2020 07:09:57 GMT  
		Size: 36.0 MB (35988813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817112d03379dcdad07585eb4a6e82d3e1667b85e534d22f6f7a0d8c311eeb89`  
		Last Modified: Tue, 13 Oct 2020 07:09:41 GMT  
		Size: 7.8 KB (7822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02bfe719cbfe70468736e03a7c4babb1da6acf32fc476b57ce71d03fa14855a`  
		Last Modified: Tue, 13 Oct 2020 07:09:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039ad490962003b676ba01db46e0b51cab4d14ff92dc713470c05550068dee0`  
		Last Modified: Tue, 13 Oct 2020 07:09:42 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb143944f126a84cc5f47cfbc47021c682ac791b819c53d37873ed9d9299498a`  
		Last Modified: Tue, 13 Oct 2020 07:09:41 GMT  
		Size: 4.3 KB (4271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62beab1da1ded61fee3aaa7c67b1485ce9e574ea95e6080fbe281f0accb54db`  
		Last Modified: Tue, 13 Oct 2020 07:09:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:75d9d3599512774ce0fbda12f358c43d881019fb5164676c10b1f488e336fea5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69726903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d87cdf01f2245f4284f78ce45d3058bd7fa65d41c9905d69b5c2e8c4803fb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:21 GMT
ADD file:1783101ec41dba711940487fb45a9287f74a0639658051ad8bc9b2618a15be61 in / 
# Tue, 13 Oct 2020 01:44:22 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:04:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 11:04:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 11:04:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 11:04:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 11:05:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 11:05:06 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 11:05:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:05:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 11:05:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 11:42:37 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 11:42:38 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 12:00:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:00:17 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:00:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:00:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 12:00:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:00:23 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:00:23 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:00:24 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:00:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:00:27 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:00:28 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:00:29 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f4bec48cdb322f1180477bdd362bcd92d70a1ab628fc36319017bf4e8058d9ee`  
		Last Modified: Tue, 13 Oct 2020 01:51:12 GMT  
		Size: 20.4 MB (20376997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984be4b3fed9808b066a7600d2e83efbfd0ff4bfc1069a9d0814be2fd022f357`  
		Last Modified: Tue, 13 Oct 2020 12:20:59 GMT  
		Size: 4.1 MB (4078528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859bbaaf4e29eade0fbd81b43a64e5eb25198a55ef466f821ac3ba984a0bab4`  
		Last Modified: Tue, 13 Oct 2020 12:20:57 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882cfdcc3440ef89e60ecc554c9e53baa9bbbc241e2b37005dcd3d8f1faabdc9`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 1.3 MB (1346994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a8ef2ba5300bad73627e9166d141b0a67a7ad8d42cb3453893fb5f5813dea`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 6.2 MB (6185301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652a08bb6feda1aad8370161437fc26c9908787e595304676ceb34feafbbe901`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 377.9 KB (377937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17111fdbd30125a36e0c8429df7d3ff1c54dfe90c2c0999e2f3738dc89019f00`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed1a1a2b06a19d02a8d4d5890f949a8a250c418de647be680f045f2240fd2e3`  
		Last Modified: Tue, 13 Oct 2020 12:20:51 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4910b3402f81c9ae1340831f481af830be486b180329daf77a1f0ea105e58b57`  
		Last Modified: Tue, 13 Oct 2020 12:21:45 GMT  
		Size: 37.3 MB (37341299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24004df8e6f8945508eb8748b24cbbf03884b06660cd737ba718638f9e2f4ec3`  
		Last Modified: Tue, 13 Oct 2020 12:21:32 GMT  
		Size: 7.8 KB (7822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0cc13302ff968f957335ee9b4b13bc241fbc046600de5b15b729f753648447`  
		Last Modified: Tue, 13 Oct 2020 12:21:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc132a52681c0ef5bdf4906668d773b46f31d8d8c78508697bf31f17cf030fe0`  
		Last Modified: Tue, 13 Oct 2020 12:21:32 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152bb52c9a6014fab6a95aed00ef73acb7e0a86c04ae4941f3bfb56c095531a`  
		Last Modified: Tue, 13 Oct 2020 12:21:32 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d4875a0d2d21c0855a002a0efcab78b3b45d1b26c21ee9032593e7f88b6b78`  
		Last Modified: Tue, 13 Oct 2020 12:21:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9` - linux; 386

```console
$ docker pull postgres@sha256:89f25789c40f514e185d374b78c0a99789b6c6155528ddf98d204114fb7ad68e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74649046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ad6d1452486390cfa2601ade7f37092954319d0322f19c9f8670622a3a6fa40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:45:31 GMT
ADD file:f09276bb607e6d68dcb997c1e8b4d004b91548964306d6a803286ba851484579 in / 
# Tue, 13 Oct 2020 01:45:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 16:43:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 16:43:18 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 16:43:18 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 16:43:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 16:43:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 16:43:49 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 16:43:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:43:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 16:44:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 16:45:33 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 16:45:34 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 16:45:58 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 16:46:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 16:46:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 16:46:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 16:46:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 16:46:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 16:46:03 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 16:46:04 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 16:46:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 16:46:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 16:46:05 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 16:46:06 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 16:46:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:02448e4a5fa68035acff67a00ba04305cbad42b25ffeb4b141c5f1f0b9d63a2a`  
		Last Modified: Tue, 13 Oct 2020 01:52:11 GMT  
		Size: 23.1 MB (23148149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1707623e5e9b92a3f43f1910a43ad9872060b853d07ecbf2b9b5bc02300501`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 4.8 MB (4809899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7908ca805e2bd89c5f1fe55e4f313469b7d84f6d049e59bc673439f8323b1d`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebde576b2c220dc444db8fcec0278f11a1df5bce6d091728aa378f74bb22734e`  
		Last Modified: Tue, 13 Oct 2020 16:48:40 GMT  
		Size: 1.4 MB (1382391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f9c2ca0b45e9e11f84e7f98ba02d277d65687fd873580517a5f0e50e6d7aac`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 6.2 MB (6182990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd5fdfe0405da8b45de435a650073673e910b7bd9545f2a05811eed28824401`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 393.2 KB (393233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3263197a4dd54e9fefd6e411e83b19f4186837e5aa15ce30c389245a5f7ae727`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1249d81ef1b333d5c1caf34a641e9466c3351724f2e669c983df59e95e4571`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cb992204d41780dd5f7549b925be4259b54f02011aa110e5f821b86b015b4f`  
		Last Modified: Tue, 13 Oct 2020 16:49:48 GMT  
		Size: 38.7 MB (38712644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d661bcbdd68df335fdb7f2d720abe429499da446f9c3d427b25b3274f0781c5`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 7.8 KB (7817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99222675c4cf88c0b967aced535ff601d8a482a42a7495ddfa6d728ab3a39e81`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402f725ca367f9c97e74d65efe05835efd19efa09809d5c7a957d68f4fd75621`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82634d7876f77a3cea0b872d3171936ca46e7fc2ee9fc494e088fcac14126810`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e898b8d6424ec432b7f46e8d86cd9a88f90958808c82e82632ad3784e8b084`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.5`

```console
$ docker pull postgres@sha256:6b5495fb6ad188dd56e8f0ed71b7dd46ea10b6b2cb01e198022689d693519fe2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:9.5` - linux; amd64

```console
$ docker pull postgres@sha256:fc311693cce62a483477df07cd9b15c5be8cbe1c40c70af385d803acd2d2d7f2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72496948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e664c45255213c5e6e7f4d57392db6fcfd53b57c0e46bb3dc94555c478a0bce5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:33:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:33:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:33:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:33:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:34:01 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:34:02 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:34:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:34:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:34:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:36:32 GMT
ENV PG_MAJOR=9.5
# Tue, 13 Oct 2020 12:36:32 GMT
ENV PG_VERSION=9.5.23-1.pgdg90+1
# Tue, 13 Oct 2020 12:36:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:36:56 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:36:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:36:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Tue, 13 Oct 2020 12:36:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:36:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:36:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:36:59 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:37:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:37:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:37:00 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:37:01 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:37:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0526c44df6ea5bd7668eab6d9c37d43aef6474cb4f5b6d2539e82404a3827041`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 4.5 MB (4502050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2466ee00e96ac149c287cdd533cecad2907d0aea2f2fe5ffc7a706ab313aaac`  
		Last Modified: Tue, 13 Oct 2020 12:38:27 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c605d60192c83f6a890b4f0cfaf8d80cf2a7a5c0c8df01451a106305748bf2`  
		Last Modified: Tue, 13 Oct 2020 12:38:28 GMT  
		Size: 1.4 MB (1412112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b14ab418421f0d1e9fb147720201f216050e2ad983640a446e75249e84e9bc`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 6.2 MB (6182797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f557fff31511f1f9475342998e8b195c0942480fb4901dab214f015d2224c`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 384.9 KB (384916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bba27806f46c2448fe4d5a0b248fd9178ced6163b8e2154e4b06a86c9a08b4`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e1555090548b1ab5739971b4eea16b502cc1e625f3a0b827463c4ae69bcc61`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53231aef374b2910d758831fd10835dd2b471c2c9f6006c64ac70669a30c852`  
		Last Modified: Tue, 13 Oct 2020 12:39:33 GMT  
		Size: 37.5 MB (37473521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac4470dcc78e0665ca58e67e6bf7e023582569664b7be2e431bba37bb9c6591`  
		Last Modified: Tue, 13 Oct 2020 12:39:22 GMT  
		Size: 7.5 KB (7528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2160506d8002a5aec200b6c7776a2be72f2afa506417e5c8c9e03a39d277713`  
		Last Modified: Tue, 13 Oct 2020 12:39:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13665ac9ebb4f66426476dc6d86eccece98defe669e5bec476836f1634ddee13`  
		Last Modified: Tue, 13 Oct 2020 12:39:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3b9fe66d69d38481d2d8584d19726e317754bd09af989a6ed5f91ed83ed06c`  
		Last Modified: Tue, 13 Oct 2020 12:39:22 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8678360b080e2ff4cad4d1ffe2777f2fb2b09b74fc9e08c70891d6941103b9`  
		Last Modified: Tue, 13 Oct 2020 12:39:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; arm variant v5

```console
$ docker pull postgres@sha256:3c27594330e5b96bdda00c1415f33afa9c23a95ef097db4c3522c45676a7ca88
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69430692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cbb0483e9adc50f8258eea00412adfb0eab5b135026d08b3213cb2c15cdcb74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:57:28 GMT
ADD file:ef761876435f34dd5e73f6fb89eda5cee26b26d9183a37dc5588c6eb5fd4ba69 in / 
# Tue, 13 Oct 2020 01:57:29 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 07:10:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 07:10:23 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 07:10:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 07:11:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 07:11:15 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 07:11:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:11:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 07:11:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 08:16:09 GMT
ENV PG_MAJOR=9.5
# Tue, 13 Oct 2020 08:16:10 GMT
ENV PG_VERSION=9.5.23-1.pgdg90+1
# Tue, 13 Oct 2020 08:35:20 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 08:35:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 08:35:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 08:35:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Tue, 13 Oct 2020 08:35:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 08:35:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 08:35:35 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 08:35:36 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:35:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 08:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:35:40 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 08:35:42 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 08:35:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e6fa5ab8c49c07aa49f655f00f7742fc2640bec642d3e0b440a9d67c37d1383e`  
		Last Modified: Tue, 13 Oct 2020 02:05:36 GMT  
		Size: 21.2 MB (21194476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4a7d58f9de066b4eb914552800ca9b9c3bdbd3a49d22592a568fd65353b60e`  
		Last Modified: Tue, 13 Oct 2020 08:37:11 GMT  
		Size: 4.2 MB (4238677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d9d67c7f2447a0677783317716fd66e891874c5dec4c300963bdaedef3db73`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8dfd96a4ee2041e6cf18fbfb05eaaf56b746f396297762c746643158da072a`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.4 MB (1371374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55137faf878bb43f0e314a0845bb679c3834709fb30668a8a966d3ea7d6324c6`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 6.2 MB (6185655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c626e10cc735d164b870d78d396556ebae2e833924a9782fc8880333228fea`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 385.1 KB (385110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5193a2411b31608c76d06bf9efa210a7cf0d1b51953e39d3cdc458342b259a86`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71923a948044364e5093b7b7e4e2667ee46f8e6fc34ff01d72050cd7aefbe702`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 5.3 KB (5350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b83e04a4929c24b11bf2a6f7587c47de0fb237dcd30238f407dbe88179f275`  
		Last Modified: Tue, 13 Oct 2020 08:38:31 GMT  
		Size: 36.0 MB (36035838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791adf4a22e35a5ca7186592dbc66008e6b19f7c8ada32400457d321e954644a`  
		Last Modified: Tue, 13 Oct 2020 08:38:16 GMT  
		Size: 7.5 KB (7534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8d761b98547b42e83c47e94be64250759c0a29c04ab229ce24055dfb30e981`  
		Last Modified: Tue, 13 Oct 2020 08:38:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83397c231724c8947796ac9e0bd59d630328a3402c79e8579138f4e8872e90b5`  
		Last Modified: Tue, 13 Oct 2020 08:38:16 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a899a2e00c85a63823b2ad6e51309735d2ed94c70be49625a4cd9be230e2a7e0`  
		Last Modified: Tue, 13 Oct 2020 08:38:16 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a04935fc6c69995df6962fa6e494170f2088983fc192bcf3bce7216f3e3f00`  
		Last Modified: Tue, 13 Oct 2020 08:38:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; arm variant v7

```console
$ docker pull postgres@sha256:dc8f9d6005760a4c404a6cb1fd16a6ca7714ab0fbb294eac6b85b1df80129f85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66137599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dacbc11dc8b49c5fb854909925bedd4a83c91ceca739258d154b72fb7b3130ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:04:30 GMT
ADD file:d204a257433edcd6f9ddd2c769b9e187c408eb4972203a5daab60214b5b576bc in / 
# Tue, 13 Oct 2020 01:04:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:54:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:54:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:54:44 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:55:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:55:24 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:55:25 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:55:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:55:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:55:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 06:50:38 GMT
ENV PG_MAJOR=9.5
# Tue, 13 Oct 2020 06:50:41 GMT
ENV PG_VERSION=9.5.23-1.pgdg90+1
# Tue, 13 Oct 2020 07:07:01 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 07:07:06 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 07:07:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 07:07:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Tue, 13 Oct 2020 07:07:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 07:07:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 07:07:14 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 07:07:15 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 07:07:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 07:07:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 07:07:20 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 07:07:20 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 07:07:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cc11be355171b10881b3ed16be16ceb2d7787cd459c6489d83bac55ee5824b35`  
		Last Modified: Tue, 13 Oct 2020 01:12:46 GMT  
		Size: 19.3 MB (19304540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8b70af887483c86f21ffd35a2a331fbab0ae0804a4929517360da6207fe6c3`  
		Last Modified: Tue, 13 Oct 2020 07:09:01 GMT  
		Size: 3.9 MB (3874946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09233e1347145a65db2aae548df648e91df34bde91664ac04509ff8ba2d77447`  
		Last Modified: Tue, 13 Oct 2020 07:08:59 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a09c7350562aee4559820b5fa1133618b8c02e7848e0c14635fb483b5a10fb`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 1.4 MB (1363819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9deba20fbd610072e97a51ac7766bcfdac37c6110ee53cdf296e7435868b5e7`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 6.2 MB (6185495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a750e8984fdec76cc5aa76a7979cd403c03d5b18efe690ebda5984356654554`  
		Last Modified: Tue, 13 Oct 2020 07:08:58 GMT  
		Size: 379.2 KB (379196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bd92fced2d524fc75c7429ca11a3f1c30587399ca0a571b4f623a3db6c15c2`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059b3634dc4169b9d362c9bf8d29e4c9af7a58bd40538452efeb506841942fb4`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208dc2f593b32aac9770e1272bb6c844e77e015249f04a09522d2435c711667`  
		Last Modified: Tue, 13 Oct 2020 07:10:19 GMT  
		Size: 35.0 MB (35010039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37acb1f9bfe3c9356bdfd67fdce1f2e5447703517ef9fa13914d612ddb51397`  
		Last Modified: Tue, 13 Oct 2020 07:10:06 GMT  
		Size: 7.5 KB (7534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d708e462ba2dc3f28ab6b78a99d600161263af284ef0dd23d3e24fe626455`  
		Last Modified: Tue, 13 Oct 2020 07:10:06 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17ccd8124c94814a3364798b84f7cf61152a02ffade932ed16a874060201d5d`  
		Last Modified: Tue, 13 Oct 2020 07:10:06 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59844797c88bacf93db0defc27241e032150c5548a7dd17c47bfaa3097731d25`  
		Last Modified: Tue, 13 Oct 2020 07:10:06 GMT  
		Size: 4.3 KB (4273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e623e4a13d77f5795a9b7a1f18ad0473b3ce64f0b65dab0debacaf782782726`  
		Last Modified: Tue, 13 Oct 2020 07:10:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:cdb24acbe19648311c5e425b531e15a79e4687bd31f8fe9270872eb4e3073e22
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.7 MB (68727167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3f42efafb4c02724dd5c63a1962f03bec25897d947187f41e58d6d36e3d51e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:21 GMT
ADD file:1783101ec41dba711940487fb45a9287f74a0639658051ad8bc9b2618a15be61 in / 
# Tue, 13 Oct 2020 01:44:22 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:04:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 11:04:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 11:04:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 11:04:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 11:05:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 11:05:06 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 11:05:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:05:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 11:05:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:00:55 GMT
ENV PG_MAJOR=9.5
# Tue, 13 Oct 2020 12:00:56 GMT
ENV PG_VERSION=9.5.23-1.pgdg90+1
# Tue, 13 Oct 2020 12:18:01 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:18:05 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:18:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:18:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Tue, 13 Oct 2020 12:18:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:18:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:18:35 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:18:37 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:18:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:18:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:18:55 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:18:56 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:18:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f4bec48cdb322f1180477bdd362bcd92d70a1ab628fc36319017bf4e8058d9ee`  
		Last Modified: Tue, 13 Oct 2020 01:51:12 GMT  
		Size: 20.4 MB (20376997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984be4b3fed9808b066a7600d2e83efbfd0ff4bfc1069a9d0814be2fd022f357`  
		Last Modified: Tue, 13 Oct 2020 12:20:59 GMT  
		Size: 4.1 MB (4078528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859bbaaf4e29eade0fbd81b43a64e5eb25198a55ef466f821ac3ba984a0bab4`  
		Last Modified: Tue, 13 Oct 2020 12:20:57 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882cfdcc3440ef89e60ecc554c9e53baa9bbbc241e2b37005dcd3d8f1faabdc9`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 1.3 MB (1346994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a8ef2ba5300bad73627e9166d141b0a67a7ad8d42cb3453893fb5f5813dea`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 6.2 MB (6185301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652a08bb6feda1aad8370161437fc26c9908787e595304676ceb34feafbbe901`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 377.9 KB (377937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17111fdbd30125a36e0c8429df7d3ff1c54dfe90c2c0999e2f3738dc89019f00`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed1a1a2b06a19d02a8d4d5890f949a8a250c418de647be680f045f2240fd2e3`  
		Last Modified: Tue, 13 Oct 2020 12:20:51 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1976b0a9bcbe0e78a9b9853c61a7f78237addd57ab773b8dcd1dbffe3b2f9b14`  
		Last Modified: Tue, 13 Oct 2020 12:22:07 GMT  
		Size: 36.3 MB (36341851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf879e992c8bf99b8addb732058d59118185aeb4591fd6f1474fb641b2ecf19`  
		Last Modified: Tue, 13 Oct 2020 12:21:54 GMT  
		Size: 7.5 KB (7533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4b0f93adf639917dd5deb880b6daacf51e05877ae42445ce82563fcd9af993`  
		Last Modified: Tue, 13 Oct 2020 12:21:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deec075d89edb01b82b20901c6e9b781322b7ada14d55ef85032e7590b617b24`  
		Last Modified: Tue, 13 Oct 2020 12:21:54 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5630202b81bd192e95de97e63aae9ea806612b0461323d14757b8a00e86d0980`  
		Last Modified: Tue, 13 Oct 2020 12:21:54 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8269702adf479f03c7f75e3cfc28692b06766034759de7cb6e8a5238160a5837`  
		Last Modified: Tue, 13 Oct 2020 12:21:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5` - linux; 386

```console
$ docker pull postgres@sha256:fe3eb54017eb1e42e0c15387b5cb1504b8ee993a8d81bdd3425ac917f8bbb769
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73625282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cff889326f19ae33a8e6c9b9b64c3adcfb1fef903e758c4100debd46df46073`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:45:31 GMT
ADD file:f09276bb607e6d68dcb997c1e8b4d004b91548964306d6a803286ba851484579 in / 
# Tue, 13 Oct 2020 01:45:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 16:43:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 16:43:18 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 16:43:18 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 16:43:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 16:43:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 16:43:49 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 16:43:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:43:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 16:44:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 16:46:19 GMT
ENV PG_MAJOR=9.5
# Tue, 13 Oct 2020 16:46:19 GMT
ENV PG_VERSION=9.5.23-1.pgdg90+1
# Tue, 13 Oct 2020 16:46:44 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 16:46:46 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 16:46:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 16:46:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.5/bin
# Tue, 13 Oct 2020 16:46:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 16:46:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 16:46:49 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 16:46:49 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 16:46:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 16:46:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 16:46:51 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 16:46:51 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 16:46:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:02448e4a5fa68035acff67a00ba04305cbad42b25ffeb4b141c5f1f0b9d63a2a`  
		Last Modified: Tue, 13 Oct 2020 01:52:11 GMT  
		Size: 23.1 MB (23148149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1707623e5e9b92a3f43f1910a43ad9872060b853d07ecbf2b9b5bc02300501`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 4.8 MB (4809899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7908ca805e2bd89c5f1fe55e4f313469b7d84f6d049e59bc673439f8323b1d`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebde576b2c220dc444db8fcec0278f11a1df5bce6d091728aa378f74bb22734e`  
		Last Modified: Tue, 13 Oct 2020 16:48:40 GMT  
		Size: 1.4 MB (1382391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f9c2ca0b45e9e11f84e7f98ba02d277d65687fd873580517a5f0e50e6d7aac`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 6.2 MB (6182990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd5fdfe0405da8b45de435a650073673e910b7bd9545f2a05811eed28824401`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 393.2 KB (393233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3263197a4dd54e9fefd6e411e83b19f4186837e5aa15ce30c389245a5f7ae727`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1249d81ef1b333d5c1caf34a641e9466c3351724f2e669c983df59e95e4571`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42dbee2f385e526cc94ac5972e9e14777d8b36c92132f4bddd90ef4fc320758`  
		Last Modified: Tue, 13 Oct 2020 16:50:08 GMT  
		Size: 37.7 MB (37689166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ecdb699a1a7c029aa66b46daee7b845ba452732edb8fa1f89db654bd5d062a`  
		Last Modified: Tue, 13 Oct 2020 16:49:55 GMT  
		Size: 7.5 KB (7529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e61a4773fd57fcf66ac266ac270b77ed814a97c58973bbcec960aab2568b29`  
		Last Modified: Tue, 13 Oct 2020 16:49:55 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b362331093702c547fc853a510049b71c734f2300fffbf7246fe23182fd59eee`  
		Last Modified: Tue, 13 Oct 2020 16:49:55 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235f95a4cc1e382732b6ff05cc9b71ca95f6f8796eff54da108dac452962069`  
		Last Modified: Tue, 13 Oct 2020 16:49:55 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41b44c534ebfc74e09f2c1059efa65bfffcb015a2dc8b47428afce176ec7fc7`  
		Last Modified: Tue, 13 Oct 2020 16:49:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.5.24`

**does not exist** (yet?)

## `postgres:9.5.24-alpine`

**does not exist** (yet?)

## `postgres:9.5-alpine`

```console
$ docker pull postgres@sha256:8ed160d0718257f4df2bb72633ec2710977241d95014865486a64620d983bcd5
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
$ docker pull postgres@sha256:fb650cb8c864250f1cd2f49c86342a582aa2a2f7da80da975242b4085502aeda
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14027039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80697e56047452e3e644d96dc7106118bd7b705d41a775af7120d5d1ffae3b69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:55:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 07:55:14 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 07:55:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:18:49 GMT
ENV PG_MAJOR=9.5
# Thu, 22 Oct 2020 08:18:49 GMT
ENV PG_VERSION=9.5.23
# Thu, 22 Oct 2020 08:18:49 GMT
ENV PG_SHA256=e314fa7e3355c4b8a35e94eeb8e58a6cf46adf49a2f9afa0c15cbc39980c8366
# Thu, 22 Oct 2020 08:21:25 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:21:26 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:21:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:21:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:21:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:21:28 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:21:28 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:21:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:21:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:21:29 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:21:30 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:21:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f1d1b70e7fa650fd6229086120f763219adce9e33e8b20bdfbf8452ab69847`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4f01476d2b86761cdb0414c4a583b89af3b5d0b67022cfc0d378743307f7e3`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58698a2c398c9bb88abe0c26a14ae1f13543f277c45984a3fb84ff78db534ed`  
		Last Modified: Thu, 22 Oct 2020 08:23:13 GMT  
		Size: 11.2 MB (11217257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37081e92ca52630d764e5276da75fe232fb1a964fa5c4d0efaa94b8854c60a50`  
		Last Modified: Thu, 22 Oct 2020 08:23:10 GMT  
		Size: 6.9 KB (6885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d365d0c77d61c91f17bb6d46caec838c4b633479893414e1cb9642cffd7908`  
		Last Modified: Thu, 22 Oct 2020 08:23:09 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d913cc1f9cc6de0ec1d6b93d6636510153e532e22c4dca0d1f11d842bc97e9da`  
		Last Modified: Thu, 22 Oct 2020 08:23:09 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fe84a238158e430744fb5c8be871e5f8dc4ad3d036802fb6c223eeb563b972`  
		Last Modified: Thu, 22 Oct 2020 08:23:09 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb5a7f7f7d7b87b325450ee36825d8e1d9a1fbca4ce29c93f475372a241270c`  
		Last Modified: Thu, 22 Oct 2020 08:23:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:ba8a7e995482b39725b78d3bccb4939a369b64e3e4390d601acd5cfb1e21234b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13398181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffb93134823ee949b692d933f679193ee33913c43d3c1e269eae8dad56a615f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:55:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:55:00 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:55:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:16:03 GMT
ENV PG_MAJOR=9.5
# Thu, 22 Oct 2020 09:16:05 GMT
ENV PG_VERSION=9.5.23
# Thu, 22 Oct 2020 09:16:07 GMT
ENV PG_SHA256=e314fa7e3355c4b8a35e94eeb8e58a6cf46adf49a2f9afa0c15cbc39980c8366
# Thu, 22 Oct 2020 09:18:37 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:18:40 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:18:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:18:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:18:46 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:18:48 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:18:50 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:18:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:18:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:18:55 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:18:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54bc8a79538fa79db3e734327f2a73654bc80285dc55b7e4d8d206161ec79a9`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30574d1822b9e42c2a6da5e4a8f52ab65d88be941e497b4565382967ebd326f8`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e15f6bc0fbc8cad1947fd706218aade4420c012b390289aee2bba72ec8dd5d4`  
		Last Modified: Thu, 22 Oct 2020 09:21:20 GMT  
		Size: 10.8 MB (10783219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507e460f607b0acf85334377705d17e2c17f291d9b4d7d2b17cef132a103f856`  
		Last Modified: Thu, 22 Oct 2020 09:21:13 GMT  
		Size: 6.9 KB (6885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb8d1f2156810fb92c9a98705af2046638157ccc8fac39456254bef876ea134`  
		Last Modified: Thu, 22 Oct 2020 09:21:13 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5309f1954198dcc66c928c4d2a3463b8649e58f53a303ca16dfcfc4d5c18139`  
		Last Modified: Thu, 22 Oct 2020 09:21:14 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e614a65c904a1085a1fe4c8f822c8c1f1572da99c149abdfe6fc51bf7aef912e`  
		Last Modified: Thu, 22 Oct 2020 09:21:14 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf0fc932cef7d9a14e992d312a545ba978c4c97745ee9d003eca51d4062fb6`  
		Last Modified: Thu, 22 Oct 2020 09:21:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:a8c930a525e222e99eb52c978dac1ad97cdc20405935c46dbc20dd0dae2a58cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.6 MB (12561800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8adc010444ab8bf42b56f4158856e2fe462d55939affccfcfd95e7fedac7edab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:56:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:56:03 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:56:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:13:41 GMT
ENV PG_MAJOR=9.5
# Thu, 22 Oct 2020 09:13:42 GMT
ENV PG_VERSION=9.5.23
# Thu, 22 Oct 2020 09:13:43 GMT
ENV PG_SHA256=e314fa7e3355c4b8a35e94eeb8e58a6cf46adf49a2f9afa0c15cbc39980c8366
# Thu, 22 Oct 2020 09:16:16 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:16:19 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:16:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:16:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:16:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:16:27 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:16:27 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:16:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:16:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:16:31 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:16:31 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:16:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7eedf40b1ca3ca0c12781ef9399626d49e7898eb4dc6bf3888a3add86c9ee2`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2cc4a27e16f2350721162545664e1c967b92e8a0ecffb90828c979f0bc3ac6`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f566ecca47905a4399aa535cf61665c5f028d1c7e953289d910123dc3c21656d`  
		Last Modified: Thu, 22 Oct 2020 09:19:04 GMT  
		Size: 10.1 MB (10143074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7b4f8538f18b44871f90a4ea2a40daa7ddfb03ab0eed4b0e9340b335279f90`  
		Last Modified: Thu, 22 Oct 2020 09:18:59 GMT  
		Size: 6.9 KB (6888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6d3e462d8e1af21ea53408eda64b2b757f7ac6636be89599a39e7d723f7aad`  
		Last Modified: Thu, 22 Oct 2020 09:18:59 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a8736e4959a14ff63b3821afe0597f3bb6a7edb4ec15b428ce793086dc5f3f`  
		Last Modified: Thu, 22 Oct 2020 09:18:59 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06774c3ec441751cef9bacaf079b5ab2602253ff447e20f37783a2a690431263`  
		Last Modified: Thu, 22 Oct 2020 09:18:59 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb921935eb04a528acbf0486929f3da6b69cd7ffd3e3df8bef39ece9637a808`  
		Last Modified: Thu, 22 Oct 2020 09:18:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:f68f0e037c9aacfc239eef421a01ae7b55d4c9021bc52ac998562dabc89fe82c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13777173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b77eaeaff342f25ee368e6b86bafc76f420c04338f06404084678fa15f68e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:21:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:21:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:21:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:40:39 GMT
ENV PG_MAJOR=9.5
# Thu, 22 Oct 2020 08:40:39 GMT
ENV PG_VERSION=9.5.23
# Thu, 22 Oct 2020 08:40:40 GMT
ENV PG_SHA256=e314fa7e3355c4b8a35e94eeb8e58a6cf46adf49a2f9afa0c15cbc39980c8366
# Thu, 22 Oct 2020 08:43:00 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:43:03 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:43:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:43:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:43:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:43:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:43:16 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:43:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:43:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:43:25 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:43:26 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:43:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b3b77440641e62ecc741cdb44f0f558d15c3f3b6d506be26f8c285f7a36ff`  
		Last Modified: Thu, 22 Oct 2020 08:44:00 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85615d5b5e22de086f665265885eae6f4cb41a63e5ed6910df6d0d03d0e90c5`  
		Last Modified: Thu, 22 Oct 2020 08:43:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f2c1200fe0923570c5614ce2eb895e6cd8950016aa3ce38fabafdeca271b83`  
		Last Modified: Thu, 22 Oct 2020 08:45:55 GMT  
		Size: 11.1 MB (11057573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6592b3d97dce7ff1918d541ca5082e24d01f06ce0684240ddbe0c940ed1c74`  
		Last Modified: Thu, 22 Oct 2020 08:45:50 GMT  
		Size: 6.9 KB (6880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b47b9b1ac57dbd307f31b66f7fedceaa6623053f55f0cfd0e581f90ea3607a`  
		Last Modified: Thu, 22 Oct 2020 08:45:50 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196d80b4ae7f10bf30c1dfdc48b4588162f6c8febf05f6d99ed0b88e7bbd2d4d`  
		Last Modified: Thu, 22 Oct 2020 08:45:50 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b30954f64b5b9dbd5b18669e245437635d92b05c42d5e29eda7295e8d2ec278`  
		Last Modified: Thu, 22 Oct 2020 08:45:50 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cffa7dad906979fb0919cee2a55aa983c3bd8f80240bb6e6e597468b8807a9`  
		Last Modified: Thu, 22 Oct 2020 08:45:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; 386

```console
$ docker pull postgres@sha256:b9582d03bd2754753dab497e312093a03c379a3b8931594c0a234b3ef9646915
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14643241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dff2d92dd0e64f2d4fcb1d5e67c74f9b6476b25fba1076b4ab674fa451c9b3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:38:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:38:39 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:38:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 10:16:01 GMT
ENV PG_MAJOR=9.5
# Thu, 22 Oct 2020 10:16:02 GMT
ENV PG_VERSION=9.5.23
# Thu, 22 Oct 2020 10:16:02 GMT
ENV PG_SHA256=e314fa7e3355c4b8a35e94eeb8e58a6cf46adf49a2f9afa0c15cbc39980c8366
# Thu, 22 Oct 2020 10:20:12 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 10:20:12 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 10:20:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 10:20:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 10:20:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 10:20:15 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 10:20:15 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 10:20:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 10:20:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 10:20:16 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 10:20:16 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 10:20:17 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596122efb908f979efd1794c09ae9c7a15ac0e4d53f2c181fd646d9f32565d9a`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeb7bd791d51cd161cadd22b53bd066e70998ebd55dd5ba92760d35f1ab9e8b`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d1c59e7b8d3f30aa98cbee2792edb3c973c3934013f06851c11c48fc827d28`  
		Last Modified: Thu, 22 Oct 2020 10:22:44 GMT  
		Size: 11.8 MB (11838909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760ad9dcd65cf77e30808db0fe728de853754c90c8b2592627f5dbc251c1361e`  
		Last Modified: Thu, 22 Oct 2020 10:22:40 GMT  
		Size: 6.9 KB (6886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f897c8f76cb6eb190a5f8d75c1b7fa160c1e7c1649e507fbb8fc9cee40b90117`  
		Last Modified: Thu, 22 Oct 2020 10:22:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e169999f6a19a1f6936f01e3c0a0393896daf7a511ff9f93e7a2ac58ddc97139`  
		Last Modified: Thu, 22 Oct 2020 10:22:40 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbcd6d819ea690c2ca4b01ab9345735a88964a0156ac4b925ac51282d7309a7`  
		Last Modified: Thu, 22 Oct 2020 10:22:40 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a08e4f58ab6f536048702abaf38ac8b45bf40fb9205b61d4583932856bc593`  
		Last Modified: Thu, 22 Oct 2020 10:22:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:65bb7a880d431f8d5c315cc455552bf27052a32750df0d8560cdd4778db484ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (14959713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:934d51d01fcd0a399e756e891a4bce0f1f534f83a2aa6e01b5321e78cce9c8cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 23:06:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 23:06:17 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 23:06:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 23:36:40 GMT
ENV PG_MAJOR=9.5
# Thu, 22 Oct 2020 23:36:46 GMT
ENV PG_VERSION=9.5.23
# Thu, 22 Oct 2020 23:36:51 GMT
ENV PG_SHA256=e314fa7e3355c4b8a35e94eeb8e58a6cf46adf49a2f9afa0c15cbc39980c8366
# Thu, 22 Oct 2020 23:39:23 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 23:39:35 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 23:39:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 23:39:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 23:40:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 23:40:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 23:40:09 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 23:40:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 23:40:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 23:40:30 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 23:40:38 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 23:40:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cba28bb2e7e5449306ade2eb73dd95379370b59f2eac45aa9f62aa4d376b1`  
		Last Modified: Thu, 22 Oct 2020 23:41:44 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b145001d871735701a01931a308a05fafba12a34115cac00163359d3ed8cf19`  
		Last Modified: Thu, 22 Oct 2020 23:41:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452cf14f9e87d25e87d9f3456f1ffdf5a1bce2609c3aaba2ff00c4352d3ff990`  
		Last Modified: Thu, 22 Oct 2020 23:44:25 GMT  
		Size: 12.1 MB (12143447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363652ee97429700eb18ec7154e28bb4a7a24b819407bd0775e05fe99a83fc3b`  
		Last Modified: Thu, 22 Oct 2020 23:44:17 GMT  
		Size: 6.9 KB (6884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8c85c6d1bede9fa2c33f80bea833c4d2a7d1d1ee562fd01dcd685735814d8f`  
		Last Modified: Thu, 22 Oct 2020 23:44:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b469c2176e2cd11299a03d44a80b427c6bf9a15d7ad626f8eac727de6d4ad28`  
		Last Modified: Thu, 22 Oct 2020 23:44:17 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a418c7c25dc79663fd02090bb362982644872865777b20d5cdc9bb846778bb`  
		Last Modified: Thu, 22 Oct 2020 23:44:17 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec449c97511a3deb4484f70987fc69408c1b484e036009ec85ae589f3c610d2`  
		Last Modified: Thu, 22 Oct 2020 23:44:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.5-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:ef1b1a75668c2ca82c152cc5ce11c5b4ac52f22dbfadf136d96028e9b3a807a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13615893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7f89bb6175ce62bd594396dd1dd9746f411b0c3164a8201b330c1776ecff70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:05:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:05:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:05:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:25:57 GMT
ENV PG_MAJOR=9.5
# Thu, 22 Oct 2020 09:25:57 GMT
ENV PG_VERSION=9.5.23
# Thu, 22 Oct 2020 09:25:58 GMT
ENV PG_SHA256=e314fa7e3355c4b8a35e94eeb8e58a6cf46adf49a2f9afa0c15cbc39980c8366
# Thu, 22 Oct 2020 09:28:26 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:28:29 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:28:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:28:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:28:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:28:34 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:28:34 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:28:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:28:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:28:37 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:28:38 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:28:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788b366e4c5d5f3b69b31ae06b2811fe54eb39bd4fd8b6107985f9982ab150a`  
		Last Modified: Thu, 22 Oct 2020 09:29:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eed686015d5efd53e62cc5b3f61833711a48184edf03c7d21f021b34f23095`  
		Last Modified: Thu, 22 Oct 2020 09:29:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896dd64d7e694827cde8cb9ba93b7d402e6996e459a5ebf193675aa07a4eb5b8`  
		Last Modified: Thu, 22 Oct 2020 09:30:55 GMT  
		Size: 11.0 MB (11037013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f379f0c915832a08b660b1ab8879a864bccb30e3208e57f174f2039a186b1ed`  
		Last Modified: Thu, 22 Oct 2020 09:30:51 GMT  
		Size: 6.9 KB (6887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0494660fef8cb2561c476907008b71625f95c5f3192a853090850060fc7c9933`  
		Last Modified: Thu, 22 Oct 2020 09:30:51 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a69999bcb641cad2c2721de132a0d19473e4c4969c020ec52368220e9b6801b`  
		Last Modified: Thu, 22 Oct 2020 09:30:51 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d58e5a39ed9028d1e3ae82188d0214479b19559cc21d77655872907c510f5`  
		Last Modified: Thu, 22 Oct 2020 09:30:52 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f0b7a30156c6928138491228d407ae3b83351007f719c5c36d5e54916f6588`  
		Last Modified: Thu, 22 Oct 2020 09:30:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.6`

```console
$ docker pull postgres@sha256:56b556d681143501e02f794d149213e7b04e0fde814689e8efeaba64cf5b86be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:9.6` - linux; amd64

```console
$ docker pull postgres@sha256:7e2f12cb4aac2ac43ece76a6f49a12c9600b1fd70bd8471a67aeef070c2de7c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73508700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb00980cabc0d97647ae88849823eca58fe70505addbefdf7073127f2554ce34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:33:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:33:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:33:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:33:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:34:01 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:34:02 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:34:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:34:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:34:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:35:57 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 12:35:57 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 12:36:13 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:36:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:36:15 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:36:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 12:36:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:36:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:36:18 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:36:18 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:36:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:36:20 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:36:20 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:36:21 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0526c44df6ea5bd7668eab6d9c37d43aef6474cb4f5b6d2539e82404a3827041`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 4.5 MB (4502050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2466ee00e96ac149c287cdd533cecad2907d0aea2f2fe5ffc7a706ab313aaac`  
		Last Modified: Tue, 13 Oct 2020 12:38:27 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c605d60192c83f6a890b4f0cfaf8d80cf2a7a5c0c8df01451a106305748bf2`  
		Last Modified: Tue, 13 Oct 2020 12:38:28 GMT  
		Size: 1.4 MB (1412112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b14ab418421f0d1e9fb147720201f216050e2ad983640a446e75249e84e9bc`  
		Last Modified: Tue, 13 Oct 2020 12:38:29 GMT  
		Size: 6.2 MB (6182797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440f557fff31511f1f9475342998e8b195c0942480fb4901dab214f015d2224c`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 384.9 KB (384916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bba27806f46c2448fe4d5a0b248fd9178ced6163b8e2154e4b06a86c9a08b4`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e1555090548b1ab5739971b4eea16b502cc1e625f3a0b827463c4ae69bcc61`  
		Last Modified: Tue, 13 Oct 2020 12:38:26 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228bfc35d59ec7fb6c7674ce61b84920448a676e97f868c2ef8190190af14d24`  
		Last Modified: Tue, 13 Oct 2020 12:39:16 GMT  
		Size: 38.5 MB (38484982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae6d4aade3a7a4e37446351fb71d60240d112a86381462748f324dce24ac198`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 7.8 KB (7815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d38f3152b7fdf51d67c1f9e1790a492c7db0a481733f64512417edb9753db19`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98e6187ea21bcec2504768d21903f612670c424ebf74cb3a5c4c47521de5de`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7ef009703566e3b88a5efa2d86e07bb1625e73962d31806810c1ed6aee6896`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 4.3 KB (4271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbb62021d40d5ab03a07921d007c562b870a110b52fffea952a8b278ea85457`  
		Last Modified: Tue, 13 Oct 2020 12:39:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; arm variant v5

```console
$ docker pull postgres@sha256:ca7856a8accf79f12b00ac75d43ac2370f94bb915376c326b36b298776d22bae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70430486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0b6923e37593fae3669f514ff41c7acd2072dc9e8453088c77777811de62c79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:57:28 GMT
ADD file:ef761876435f34dd5e73f6fb89eda5cee26b26d9183a37dc5588c6eb5fd4ba69 in / 
# Tue, 13 Oct 2020 01:57:29 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 07:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 07:10:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 07:10:23 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 07:10:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 07:11:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 07:11:15 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 07:11:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 07:11:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 07:11:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 07:55:24 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 07:55:25 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 08:15:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 08:15:45 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 08:15:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 08:15:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 08:15:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 08:15:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 08:15:53 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 08:15:54 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:15:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 08:15:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:15:58 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 08:15:59 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 08:16:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e6fa5ab8c49c07aa49f655f00f7742fc2640bec642d3e0b440a9d67c37d1383e`  
		Last Modified: Tue, 13 Oct 2020 02:05:36 GMT  
		Size: 21.2 MB (21194476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4a7d58f9de066b4eb914552800ca9b9c3bdbd3a49d22592a568fd65353b60e`  
		Last Modified: Tue, 13 Oct 2020 08:37:11 GMT  
		Size: 4.2 MB (4238677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d9d67c7f2447a0677783317716fd66e891874c5dec4c300963bdaedef3db73`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8dfd96a4ee2041e6cf18fbfb05eaaf56b746f396297762c746643158da072a`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 1.4 MB (1371374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55137faf878bb43f0e314a0845bb679c3834709fb30668a8a966d3ea7d6324c6`  
		Last Modified: Tue, 13 Oct 2020 08:37:09 GMT  
		Size: 6.2 MB (6185655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c626e10cc735d164b870d78d396556ebae2e833924a9782fc8880333228fea`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 385.1 KB (385110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5193a2411b31608c76d06bf9efa210a7cf0d1b51953e39d3cdc458342b259a86`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71923a948044364e5093b7b7e4e2667ee46f8e6fc34ff01d72050cd7aefbe702`  
		Last Modified: Tue, 13 Oct 2020 08:37:07 GMT  
		Size: 5.3 KB (5350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4c3b81731670fd755cfdb0288eba11d45531b0f20ca8403f749cfecb7b5ca`  
		Last Modified: Tue, 13 Oct 2020 08:38:06 GMT  
		Size: 37.0 MB (37035346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8090714820c2155ccec56ed8b32cc8c3f629df37306bbafb73d090290515b0af`  
		Last Modified: Tue, 13 Oct 2020 08:37:49 GMT  
		Size: 7.8 KB (7820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869ebf10e05a7071d6297a796991331fe77699ddd6c06be50a95c7915120d49e`  
		Last Modified: Tue, 13 Oct 2020 08:37:48 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6407a17dd66fe517830ebd77c7711abe5ad5e370aadad7bcbbf9b7f3a940f3`  
		Last Modified: Tue, 13 Oct 2020 08:37:48 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9f5ca54f96ae786eb52e72557dcf9a6099e3eb7ee9304e8d7d10a6b110a124`  
		Last Modified: Tue, 13 Oct 2020 08:37:48 GMT  
		Size: 4.3 KB (4273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289ab3f2ecdbf9d195a9265f32e931fa915c9c3f16234315b35d83d2c2c40008`  
		Last Modified: Tue, 13 Oct 2020 08:37:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; arm variant v7

```console
$ docker pull postgres@sha256:31b3cd029967319dc19246604401d0d6b7799479c1e93293be0a653d15a94154
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67116658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb26ab48758ca5206f2fc7b879a00a884505072b6491ef4c0693156139683c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:04:30 GMT
ADD file:d204a257433edcd6f9ddd2c769b9e187c408eb4972203a5daab60214b5b576bc in / 
# Tue, 13 Oct 2020 01:04:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:54:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:54:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:54:44 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:55:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:55:24 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:55:25 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:55:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:55:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:55:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 06:32:53 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 06:32:54 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 06:50:04 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 06:50:08 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 06:50:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 06:50:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 06:50:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 06:50:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 06:50:14 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 06:50:14 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:50:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 06:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:50:18 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 06:50:19 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 06:50:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cc11be355171b10881b3ed16be16ceb2d7787cd459c6489d83bac55ee5824b35`  
		Last Modified: Tue, 13 Oct 2020 01:12:46 GMT  
		Size: 19.3 MB (19304540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8b70af887483c86f21ffd35a2a331fbab0ae0804a4929517360da6207fe6c3`  
		Last Modified: Tue, 13 Oct 2020 07:09:01 GMT  
		Size: 3.9 MB (3874946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09233e1347145a65db2aae548df648e91df34bde91664ac04509ff8ba2d77447`  
		Last Modified: Tue, 13 Oct 2020 07:08:59 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a09c7350562aee4559820b5fa1133618b8c02e7848e0c14635fb483b5a10fb`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 1.4 MB (1363819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9deba20fbd610072e97a51ac7766bcfdac37c6110ee53cdf296e7435868b5e7`  
		Last Modified: Tue, 13 Oct 2020 07:09:00 GMT  
		Size: 6.2 MB (6185495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a750e8984fdec76cc5aa76a7979cd403c03d5b18efe690ebda5984356654554`  
		Last Modified: Tue, 13 Oct 2020 07:08:58 GMT  
		Size: 379.2 KB (379196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bd92fced2d524fc75c7429ca11a3f1c30587399ca0a571b4f623a3db6c15c2`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059b3634dc4169b9d362c9bf8d29e4c9af7a58bd40538452efeb506841942fb4`  
		Last Modified: Tue, 13 Oct 2020 07:08:57 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee03b7c7b17e1992d1b43f10c016e8fc7369f82c5d3b8d9ab28526dda9e624d`  
		Last Modified: Tue, 13 Oct 2020 07:09:57 GMT  
		Size: 36.0 MB (35988813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817112d03379dcdad07585eb4a6e82d3e1667b85e534d22f6f7a0d8c311eeb89`  
		Last Modified: Tue, 13 Oct 2020 07:09:41 GMT  
		Size: 7.8 KB (7822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02bfe719cbfe70468736e03a7c4babb1da6acf32fc476b57ce71d03fa14855a`  
		Last Modified: Tue, 13 Oct 2020 07:09:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4039ad490962003b676ba01db46e0b51cab4d14ff92dc713470c05550068dee0`  
		Last Modified: Tue, 13 Oct 2020 07:09:42 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb143944f126a84cc5f47cfbc47021c682ac791b819c53d37873ed9d9299498a`  
		Last Modified: Tue, 13 Oct 2020 07:09:41 GMT  
		Size: 4.3 KB (4271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62beab1da1ded61fee3aaa7c67b1485ce9e574ea95e6080fbe281f0accb54db`  
		Last Modified: Tue, 13 Oct 2020 07:09:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:75d9d3599512774ce0fbda12f358c43d881019fb5164676c10b1f488e336fea5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69726903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d87cdf01f2245f4284f78ce45d3058bd7fa65d41c9905d69b5c2e8c4803fb16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:21 GMT
ADD file:1783101ec41dba711940487fb45a9287f74a0639658051ad8bc9b2618a15be61 in / 
# Tue, 13 Oct 2020 01:44:22 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:04:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 11:04:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 11:04:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 11:04:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 11:05:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 11:05:06 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 11:05:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:05:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 11:05:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 11:42:37 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 11:42:38 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 12:00:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:00:17 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:00:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:00:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 12:00:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:00:23 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:00:23 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:00:24 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:00:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:00:27 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:00:28 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:00:29 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f4bec48cdb322f1180477bdd362bcd92d70a1ab628fc36319017bf4e8058d9ee`  
		Last Modified: Tue, 13 Oct 2020 01:51:12 GMT  
		Size: 20.4 MB (20376997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984be4b3fed9808b066a7600d2e83efbfd0ff4bfc1069a9d0814be2fd022f357`  
		Last Modified: Tue, 13 Oct 2020 12:20:59 GMT  
		Size: 4.1 MB (4078528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859bbaaf4e29eade0fbd81b43a64e5eb25198a55ef466f821ac3ba984a0bab4`  
		Last Modified: Tue, 13 Oct 2020 12:20:57 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882cfdcc3440ef89e60ecc554c9e53baa9bbbc241e2b37005dcd3d8f1faabdc9`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 1.3 MB (1346994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a8ef2ba5300bad73627e9166d141b0a67a7ad8d42cb3453893fb5f5813dea`  
		Last Modified: Tue, 13 Oct 2020 12:20:54 GMT  
		Size: 6.2 MB (6185301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652a08bb6feda1aad8370161437fc26c9908787e595304676ceb34feafbbe901`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 377.9 KB (377937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17111fdbd30125a36e0c8429df7d3ff1c54dfe90c2c0999e2f3738dc89019f00`  
		Last Modified: Tue, 13 Oct 2020 12:20:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed1a1a2b06a19d02a8d4d5890f949a8a250c418de647be680f045f2240fd2e3`  
		Last Modified: Tue, 13 Oct 2020 12:20:51 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4910b3402f81c9ae1340831f481af830be486b180329daf77a1f0ea105e58b57`  
		Last Modified: Tue, 13 Oct 2020 12:21:45 GMT  
		Size: 37.3 MB (37341299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24004df8e6f8945508eb8748b24cbbf03884b06660cd737ba718638f9e2f4ec3`  
		Last Modified: Tue, 13 Oct 2020 12:21:32 GMT  
		Size: 7.8 KB (7822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0cc13302ff968f957335ee9b4b13bc241fbc046600de5b15b729f753648447`  
		Last Modified: Tue, 13 Oct 2020 12:21:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc132a52681c0ef5bdf4906668d773b46f31d8d8c78508697bf31f17cf030fe0`  
		Last Modified: Tue, 13 Oct 2020 12:21:32 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8152bb52c9a6014fab6a95aed00ef73acb7e0a86c04ae4941f3bfb56c095531a`  
		Last Modified: Tue, 13 Oct 2020 12:21:32 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d4875a0d2d21c0855a002a0efcab78b3b45d1b26c21ee9032593e7f88b6b78`  
		Last Modified: Tue, 13 Oct 2020 12:21:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6` - linux; 386

```console
$ docker pull postgres@sha256:89f25789c40f514e185d374b78c0a99789b6c6155528ddf98d204114fb7ad68e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74649046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ad6d1452486390cfa2601ade7f37092954319d0322f19c9f8670622a3a6fa40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:45:31 GMT
ADD file:f09276bb607e6d68dcb997c1e8b4d004b91548964306d6a803286ba851484579 in / 
# Tue, 13 Oct 2020 01:45:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 16:43:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 16:43:18 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 16:43:18 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 16:43:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 16:43:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 16:43:49 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 16:43:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:43:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 16:44:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 16:45:33 GMT
ENV PG_MAJOR=9.6
# Tue, 13 Oct 2020 16:45:34 GMT
ENV PG_VERSION=9.6.19-1.pgdg90+1
# Tue, 13 Oct 2020 16:45:58 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 16:46:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 16:46:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 16:46:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 13 Oct 2020 16:46:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 16:46:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 16:46:03 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 16:46:04 GMT
COPY file:cfbddd6bbbc80f3e5e232700023ccabc8dc57e5080e2200436538d799fadf82e in /usr/local/bin/ 
# Tue, 13 Oct 2020 16:46:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 16:46:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 16:46:05 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 16:46:06 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 16:46:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:02448e4a5fa68035acff67a00ba04305cbad42b25ffeb4b141c5f1f0b9d63a2a`  
		Last Modified: Tue, 13 Oct 2020 01:52:11 GMT  
		Size: 23.1 MB (23148149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1707623e5e9b92a3f43f1910a43ad9872060b853d07ecbf2b9b5bc02300501`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 4.8 MB (4809899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7908ca805e2bd89c5f1fe55e4f313469b7d84f6d049e59bc673439f8323b1d`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebde576b2c220dc444db8fcec0278f11a1df5bce6d091728aa378f74bb22734e`  
		Last Modified: Tue, 13 Oct 2020 16:48:40 GMT  
		Size: 1.4 MB (1382391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f9c2ca0b45e9e11f84e7f98ba02d277d65687fd873580517a5f0e50e6d7aac`  
		Last Modified: Tue, 13 Oct 2020 16:48:42 GMT  
		Size: 6.2 MB (6182990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd5fdfe0405da8b45de435a650073673e910b7bd9545f2a05811eed28824401`  
		Last Modified: Tue, 13 Oct 2020 16:48:39 GMT  
		Size: 393.2 KB (393233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3263197a4dd54e9fefd6e411e83b19f4186837e5aa15ce30c389245a5f7ae727`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1249d81ef1b333d5c1caf34a641e9466c3351724f2e669c983df59e95e4571`  
		Last Modified: Tue, 13 Oct 2020 16:48:38 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cb992204d41780dd5f7549b925be4259b54f02011aa110e5f821b86b015b4f`  
		Last Modified: Tue, 13 Oct 2020 16:49:48 GMT  
		Size: 38.7 MB (38712644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d661bcbdd68df335fdb7f2d720abe429499da446f9c3d427b25b3274f0781c5`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 7.8 KB (7817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99222675c4cf88c0b967aced535ff601d8a482a42a7495ddfa6d728ab3a39e81`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402f725ca367f9c97e74d65efe05835efd19efa09809d5c7a957d68f4fd75621`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82634d7876f77a3cea0b872d3171936ca46e7fc2ee9fc494e088fcac14126810`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e898b8d6424ec432b7f46e8d86cd9a88f90958808c82e82632ad3784e8b084`  
		Last Modified: Tue, 13 Oct 2020 16:49:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9.6.20`

**does not exist** (yet?)

## `postgres:9.6.20-alpine`

**does not exist** (yet?)

## `postgres:9.6-alpine`

```console
$ docker pull postgres@sha256:bf8b7232f66a48cda8e3e549679fddd04d91bdbab4d728180e3dddd05a881d3d
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
$ docker pull postgres@sha256:06752892428559d9a41e93cd4d92e56cc4e82c4201651897212f8c10f6632db6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14365424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae8555aaa187b2026ab5033433f2f1e868c7733c072d309a52c77f6734295b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:55:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 07:55:14 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 07:55:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:15:43 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 08:15:44 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 08:15:44 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 08:18:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:18:29 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:18:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:18:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:18:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:18:31 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:18:31 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:18:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:18:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:18:32 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:18:32 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:18:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f1d1b70e7fa650fd6229086120f763219adce9e33e8b20bdfbf8452ab69847`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4f01476d2b86761cdb0414c4a583b89af3b5d0b67022cfc0d378743307f7e3`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179d7be7b4237214833e8ea20d0b907c21e35024318b43e6c8cd06428744050`  
		Last Modified: Thu, 22 Oct 2020 08:23:04 GMT  
		Size: 11.6 MB (11555367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29a2d8a4f2ee881e1b5ce7b32579a53c3a848438266620dc45b215c735413b7`  
		Last Modified: Thu, 22 Oct 2020 08:23:00 GMT  
		Size: 7.2 KB (7155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a172822640626694f3e853854e8fb28a20790e6225a33af195c054b906208c`  
		Last Modified: Thu, 22 Oct 2020 08:23:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055275bcb033d0e80b3af91c2f33b4fc846f81b8ccd6a057f246cdf7372d89d7`  
		Last Modified: Thu, 22 Oct 2020 08:23:00 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9de5b8b822f6bd204cfa3783e477f58c3d8207905f25c9a0845933026582c5`  
		Last Modified: Thu, 22 Oct 2020 08:23:00 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1754f690cf388dc30a24d56bd7160b9f8ad1689dd68c7c5093817f7323f823`  
		Last Modified: Thu, 22 Oct 2020 08:23:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:67d073a22cc1ecf823342968c0d242d0f4a8e7ac9290189dcad431a3a705696f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13718476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d8b35083692d61e66c3157a2a960622765bb87839169319b5b053e98be97551`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:55:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:55:00 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:55:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:12:58 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 09:12:59 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 09:13:01 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 09:15:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:15:42 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:15:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:15:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:15:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:15:47 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:15:48 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:15:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:15:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:15:51 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:15:52 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:15:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54bc8a79538fa79db3e734327f2a73654bc80285dc55b7e4d8d206161ec79a9`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30574d1822b9e42c2a6da5e4a8f52ab65d88be941e497b4565382967ebd326f8`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0353861e0ba1303d75caddfcb98a9514a897fe1ad27e9987c30a038cafbd1f84`  
		Last Modified: Thu, 22 Oct 2020 09:21:05 GMT  
		Size: 11.1 MB (11103240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce900d8cdd76c363e93b952488d855f4db7edb56bf18586738c5155f8910ace6`  
		Last Modified: Thu, 22 Oct 2020 09:21:00 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dd112bb8267e5d8120d52615ddb45fd149620202073d31cfd1c36d0a86d228`  
		Last Modified: Thu, 22 Oct 2020 09:20:59 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3a661aa047f8b6ad5f4e69ebc039a6b94736286292ec99afefc4944e9af6ca`  
		Last Modified: Thu, 22 Oct 2020 09:20:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a5519058f3c71aef9b7348fa7b0d319bb82301bc374264b0dcb8ee465ac34e`  
		Last Modified: Thu, 22 Oct 2020 09:20:59 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abfb45db984f06c99a205023cb282cf565f493ad241b33c248bc9547ffa3bd8`  
		Last Modified: Thu, 22 Oct 2020 09:20:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:5369e2dde1cc60cd45d12d0028a321560d01b1bd24d1b90262724220fc95afee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12860723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64969ad89255630ecd8302a86d3682899e4a62a17af13c7458cb08a946391ebc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:56:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:56:03 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:56:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:10:47 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 09:10:48 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 09:10:49 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 09:12:57 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:13:01 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:13:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:13:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:13:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:13:11 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:13:12 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:13:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:17 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:13:18 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:13:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7eedf40b1ca3ca0c12781ef9399626d49e7898eb4dc6bf3888a3add86c9ee2`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2cc4a27e16f2350721162545664e1c967b92e8a0ecffb90828c979f0bc3ac6`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53785c7aec3d1276ae4b10987aa89cebc8412388045f6baf9f0a637bbb0c2015`  
		Last Modified: Thu, 22 Oct 2020 09:18:50 GMT  
		Size: 10.4 MB (10441734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275f309721b4225433fc48686dbe7d6410d89807a0cdb590c1dcd5649eb484b1`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 7.2 KB (7157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e104ff37806c9fa3e5008bf545d74a33d4173f8f1579cd4928a496061498d75`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801ac3ef86690c912755d74e1c57ed17cc5c73ff9902db3609a9962433db2271`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c133a7d49e198bdd8340af20aa1857a53282f73a6f5db01dbce12364b3d0c`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb08348cca9112313ea90413d551cb1251ef4e9beca2c9aed2e728c9cf090441`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:2d9b40372db5fe833205819860b9a336edef23f5592dc26768f8cb841e66c4b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14116758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618f1d3c59515af40d2e7ec530ea2e41f81e2cbce49813b5ba350112cf4879dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:21:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:21:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:21:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:37:21 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 08:37:22 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 08:37:22 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 08:39:44 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:39:53 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:39:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:39:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:40:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:40:01 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:40:02 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:40:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:40:07 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:40:08 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:40:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b3b77440641e62ecc741cdb44f0f558d15c3f3b6d506be26f8c285f7a36ff`  
		Last Modified: Thu, 22 Oct 2020 08:44:00 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85615d5b5e22de086f665265885eae6f4cb41a63e5ed6910df6d0d03d0e90c5`  
		Last Modified: Thu, 22 Oct 2020 08:43:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8141e5be2f31b8d09929acb70098043a5aa98c1f8c86986948c37a843aaa83`  
		Last Modified: Thu, 22 Oct 2020 08:45:38 GMT  
		Size: 11.4 MB (11396878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07261327025c61b6beb447d094d66a06ed88625319d7f4c902a89cadb0d6ae8a`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da07d01698a33c72f1fb08fed9b243a446be5275b69c1ad78a06c6890d6fd25`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95aad8041870a4e76dc5a00453f1363fe25758d2a41b8c93be7fdc704bf5103d`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b21e61063dd7b2895ff5df47faff52baf9b388034c7ed66e0340f88b9a2dbc`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236756de9b740bc6ee28fb6b31caf2526a4111f3ebee1eac2def95f6b0efc012`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; 386

```console
$ docker pull postgres@sha256:1ed451a975f14d9b179c34833299ad2f2ff912b1399e5e4fda9c0673928b85af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (14989304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aac0655a0cd9bce8a679dfb01a2b0b62cda2d77d22872a3c735e020d06366ac3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:38:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:38:39 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:38:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 10:10:53 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 10:10:53 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 10:10:53 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 10:15:35 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 10:15:36 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 10:15:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 10:15:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 10:15:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 10:15:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 10:15:39 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 10:15:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 10:15:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 10:15:40 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 10:15:40 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 10:15:40 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596122efb908f979efd1794c09ae9c7a15ac0e4d53f2c181fd646d9f32565d9a`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeb7bd791d51cd161cadd22b53bd066e70998ebd55dd5ba92760d35f1ab9e8b`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1758be1146af620a798e2b4c53cd74aaf548ebe165a0a08c3fac63ffa4e86b09`  
		Last Modified: Thu, 22 Oct 2020 10:22:33 GMT  
		Size: 12.2 MB (12184704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9d90a4e11d391abfa55d9335c7ec9324a543f2163ff8a1cc125b11a2e4ef97`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa48291f0d77a0bd7e9dabdf838169179cfdc6c23857b311fa031163511c4561`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1293de77bf81d3848e5cbeeda29c1f51f8f928b1f6f1d3717abac98747855a`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7dc00f7541cb05ae4ec43b8a95d096076e6429c39978c86850d01ca7c00073`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6da5edf25e93eb293d0dc607c9a1c01b56bb4f23309a332a5d9da92f3c6171`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:a5a6dca3954a8abccc03e64d6d7de5712eba6ceaac3ce394fd9f1fd3db52f896
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15310690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37913a6c66d331d6fd59e0f0ef8f4604700f2a6be84e7d4faf27948f2b494c1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 23:06:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 23:06:17 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 23:06:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 23:32:11 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 23:32:20 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 23:32:27 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 23:35:05 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 23:35:18 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 23:35:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 23:35:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 23:35:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 23:35:57 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 23:35:59 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 23:36:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 23:36:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 23:36:20 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 23:36:25 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 23:36:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cba28bb2e7e5449306ade2eb73dd95379370b59f2eac45aa9f62aa4d376b1`  
		Last Modified: Thu, 22 Oct 2020 23:41:44 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b145001d871735701a01931a308a05fafba12a34115cac00163359d3ed8cf19`  
		Last Modified: Thu, 22 Oct 2020 23:41:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6a1a73ecd917bb30acaba74aa897d40dd155ce8c61f25c6093ebbe34a9b014`  
		Last Modified: Thu, 22 Oct 2020 23:43:59 GMT  
		Size: 12.5 MB (12494146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6f70e06b6dc89317aaec50adfd52d8f2ee7f88fe47fcbf68a5adec7c98fdad`  
		Last Modified: Thu, 22 Oct 2020 23:43:51 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d353780080303b0aaa6521d28febb7c2c906191e6a2a6ddee9b381d5298a6c4e`  
		Last Modified: Thu, 22 Oct 2020 23:43:51 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68c44ecf52e8a38cedb46f2db89186752750dca720c5aa2cfa5951a8578cc81`  
		Last Modified: Thu, 22 Oct 2020 23:43:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cf1ed629be8e282f7a83ad8c9be39033c366b806180dc40ce47368d50b1b21`  
		Last Modified: Thu, 22 Oct 2020 23:43:51 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff792e55d1b8e76fb093b3f0c59408466b080ca2e637bd47c9e8e1c4c7a984`  
		Last Modified: Thu, 22 Oct 2020 23:43:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9.6-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:043bc5a0988b5d70581f6eaf28fb4179d09924b943833a41e599e99de93d1e8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13947828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1c0a66df00471b6b7de7c17c3de326a3ebb3154f1a837ea476d1bae51d1d082`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:05:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:05:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:05:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:23:07 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 09:23:08 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 09:23:09 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 09:25:37 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:25:41 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:25:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:25:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:25:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:25:45 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:25:45 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:25:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:25:48 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:25:49 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:25:50 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788b366e4c5d5f3b69b31ae06b2811fe54eb39bd4fd8b6107985f9982ab150a`  
		Last Modified: Thu, 22 Oct 2020 09:29:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eed686015d5efd53e62cc5b3f61833711a48184edf03c7d21f021b34f23095`  
		Last Modified: Thu, 22 Oct 2020 09:29:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2502469121171c05fc2f76e2ad25767cecbc16ec44c84033ab905b36752eb0d`  
		Last Modified: Thu, 22 Oct 2020 09:30:42 GMT  
		Size: 11.4 MB (11368676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cc3be8653ac381149a46e7f166fde6a9ca653af9910e5f3d5a35264a36f29a`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b285cd8c68c9ee9e6f882198a1940aa45563fe88a8146469b79631151b7efbf`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502a91a7c371d7662208ddf836152fadf3edeff45575861591c96ca9f5208a8b`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368653c8a2e4b08c6667d3e0a3655086f876d2b4ff5010959422ab2abfb4309`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e262a0e2bb6bc8b64f64f8fe85e555c43914c92b037beb969cb3bd3117995696`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:bf8b7232f66a48cda8e3e549679fddd04d91bdbab4d728180e3dddd05a881d3d
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
$ docker pull postgres@sha256:06752892428559d9a41e93cd4d92e56cc4e82c4201651897212f8c10f6632db6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.4 MB (14365424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae8555aaa187b2026ab5033433f2f1e868c7733c072d309a52c77f6734295b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:55:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 07:55:14 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 07:55:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:15:43 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 08:15:44 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 08:15:44 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 08:18:28 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:18:29 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:18:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:18:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:18:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:18:31 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:18:31 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:18:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:18:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:18:32 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:18:32 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:18:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f1d1b70e7fa650fd6229086120f763219adce9e33e8b20bdfbf8452ab69847`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4f01476d2b86761cdb0414c4a583b89af3b5d0b67022cfc0d378743307f7e3`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179d7be7b4237214833e8ea20d0b907c21e35024318b43e6c8cd06428744050`  
		Last Modified: Thu, 22 Oct 2020 08:23:04 GMT  
		Size: 11.6 MB (11555367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29a2d8a4f2ee881e1b5ce7b32579a53c3a848438266620dc45b215c735413b7`  
		Last Modified: Thu, 22 Oct 2020 08:23:00 GMT  
		Size: 7.2 KB (7155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a172822640626694f3e853854e8fb28a20790e6225a33af195c054b906208c`  
		Last Modified: Thu, 22 Oct 2020 08:23:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055275bcb033d0e80b3af91c2f33b4fc846f81b8ccd6a057f246cdf7372d89d7`  
		Last Modified: Thu, 22 Oct 2020 08:23:00 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9de5b8b822f6bd204cfa3783e477f58c3d8207905f25c9a0845933026582c5`  
		Last Modified: Thu, 22 Oct 2020 08:23:00 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1754f690cf388dc30a24d56bd7160b9f8ad1689dd68c7c5093817f7323f823`  
		Last Modified: Thu, 22 Oct 2020 08:23:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:67d073a22cc1ecf823342968c0d242d0f4a8e7ac9290189dcad431a3a705696f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13718476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d8b35083692d61e66c3157a2a960622765bb87839169319b5b053e98be97551`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:55:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:55:00 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:55:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:12:58 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 09:12:59 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 09:13:01 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 09:15:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:15:42 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:15:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:15:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:15:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:15:47 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:15:48 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:15:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:15:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:15:51 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:15:52 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:15:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54bc8a79538fa79db3e734327f2a73654bc80285dc55b7e4d8d206161ec79a9`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30574d1822b9e42c2a6da5e4a8f52ab65d88be941e497b4565382967ebd326f8`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0353861e0ba1303d75caddfcb98a9514a897fe1ad27e9987c30a038cafbd1f84`  
		Last Modified: Thu, 22 Oct 2020 09:21:05 GMT  
		Size: 11.1 MB (11103240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce900d8cdd76c363e93b952488d855f4db7edb56bf18586738c5155f8910ace6`  
		Last Modified: Thu, 22 Oct 2020 09:21:00 GMT  
		Size: 7.2 KB (7161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dd112bb8267e5d8120d52615ddb45fd149620202073d31cfd1c36d0a86d228`  
		Last Modified: Thu, 22 Oct 2020 09:20:59 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3a661aa047f8b6ad5f4e69ebc039a6b94736286292ec99afefc4944e9af6ca`  
		Last Modified: Thu, 22 Oct 2020 09:20:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a5519058f3c71aef9b7348fa7b0d319bb82301bc374264b0dcb8ee465ac34e`  
		Last Modified: Thu, 22 Oct 2020 09:20:59 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abfb45db984f06c99a205023cb282cf565f493ad241b33c248bc9547ffa3bd8`  
		Last Modified: Thu, 22 Oct 2020 09:20:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:5369e2dde1cc60cd45d12d0028a321560d01b1bd24d1b90262724220fc95afee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12860723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64969ad89255630ecd8302a86d3682899e4a62a17af13c7458cb08a946391ebc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:56:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:56:03 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:56:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:10:47 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 09:10:48 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 09:10:49 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 09:12:57 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:13:01 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:13:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:13:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:13:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:13:11 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:13:12 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:13:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:13:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:13:17 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:13:18 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:13:19 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7eedf40b1ca3ca0c12781ef9399626d49e7898eb4dc6bf3888a3add86c9ee2`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2cc4a27e16f2350721162545664e1c967b92e8a0ecffb90828c979f0bc3ac6`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53785c7aec3d1276ae4b10987aa89cebc8412388045f6baf9f0a637bbb0c2015`  
		Last Modified: Thu, 22 Oct 2020 09:18:50 GMT  
		Size: 10.4 MB (10441734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275f309721b4225433fc48686dbe7d6410d89807a0cdb590c1dcd5649eb484b1`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 7.2 KB (7157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e104ff37806c9fa3e5008bf545d74a33d4173f8f1579cd4928a496061498d75`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801ac3ef86690c912755d74e1c57ed17cc5c73ff9902db3609a9962433db2271`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776c133a7d49e198bdd8340af20aa1857a53282f73a6f5db01dbce12364b3d0c`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb08348cca9112313ea90413d551cb1251ef4e9beca2c9aed2e728c9cf090441`  
		Last Modified: Thu, 22 Oct 2020 09:18:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:2d9b40372db5fe833205819860b9a336edef23f5592dc26768f8cb841e66c4b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14116758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618f1d3c59515af40d2e7ec530ea2e41f81e2cbce49813b5ba350112cf4879dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:21:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:21:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:21:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:37:21 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 08:37:22 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 08:37:22 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 08:39:44 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:39:53 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:39:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:39:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:40:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:40:01 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:40:02 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:40:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 08:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:40:07 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:40:08 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:40:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b3b77440641e62ecc741cdb44f0f558d15c3f3b6d506be26f8c285f7a36ff`  
		Last Modified: Thu, 22 Oct 2020 08:44:00 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85615d5b5e22de086f665265885eae6f4cb41a63e5ed6910df6d0d03d0e90c5`  
		Last Modified: Thu, 22 Oct 2020 08:43:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8141e5be2f31b8d09929acb70098043a5aa98c1f8c86986948c37a843aaa83`  
		Last Modified: Thu, 22 Oct 2020 08:45:38 GMT  
		Size: 11.4 MB (11396878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07261327025c61b6beb447d094d66a06ed88625319d7f4c902a89cadb0d6ae8a`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da07d01698a33c72f1fb08fed9b243a446be5275b69c1ad78a06c6890d6fd25`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95aad8041870a4e76dc5a00453f1363fe25758d2a41b8c93be7fdc704bf5103d`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b21e61063dd7b2895ff5df47faff52baf9b388034c7ed66e0340f88b9a2dbc`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236756de9b740bc6ee28fb6b31caf2526a4111f3ebee1eac2def95f6b0efc012`  
		Last Modified: Thu, 22 Oct 2020 08:45:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; 386

```console
$ docker pull postgres@sha256:1ed451a975f14d9b179c34833299ad2f2ff912b1399e5e4fda9c0673928b85af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (14989304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aac0655a0cd9bce8a679dfb01a2b0b62cda2d77d22872a3c735e020d06366ac3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:38:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:38:39 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:38:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 10:10:53 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 10:10:53 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 10:10:53 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 10:15:35 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 10:15:36 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 10:15:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 10:15:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 10:15:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 10:15:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 10:15:39 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 10:15:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 10:15:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 10:15:40 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 10:15:40 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 10:15:40 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596122efb908f979efd1794c09ae9c7a15ac0e4d53f2c181fd646d9f32565d9a`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeb7bd791d51cd161cadd22b53bd066e70998ebd55dd5ba92760d35f1ab9e8b`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1758be1146af620a798e2b4c53cd74aaf548ebe165a0a08c3fac63ffa4e86b09`  
		Last Modified: Thu, 22 Oct 2020 10:22:33 GMT  
		Size: 12.2 MB (12184704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9d90a4e11d391abfa55d9335c7ec9324a543f2163ff8a1cc125b11a2e4ef97`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa48291f0d77a0bd7e9dabdf838169179cfdc6c23857b311fa031163511c4561`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1293de77bf81d3848e5cbeeda29c1f51f8f928b1f6f1d3717abac98747855a`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7dc00f7541cb05ae4ec43b8a95d096076e6429c39978c86850d01ca7c00073`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6da5edf25e93eb293d0dc607c9a1c01b56bb4f23309a332a5d9da92f3c6171`  
		Last Modified: Thu, 22 Oct 2020 10:22:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:a5a6dca3954a8abccc03e64d6d7de5712eba6ceaac3ce394fd9f1fd3db52f896
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15310690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37913a6c66d331d6fd59e0f0ef8f4604700f2a6be84e7d4faf27948f2b494c1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 23:06:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 23:06:17 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 23:06:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 23:32:11 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 23:32:20 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 23:32:27 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 23:35:05 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 23:35:18 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 23:35:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 23:35:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 23:35:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 23:35:57 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 23:35:59 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 23:36:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 23:36:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 23:36:20 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 23:36:25 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 23:36:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cba28bb2e7e5449306ade2eb73dd95379370b59f2eac45aa9f62aa4d376b1`  
		Last Modified: Thu, 22 Oct 2020 23:41:44 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b145001d871735701a01931a308a05fafba12a34115cac00163359d3ed8cf19`  
		Last Modified: Thu, 22 Oct 2020 23:41:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6a1a73ecd917bb30acaba74aa897d40dd155ce8c61f25c6093ebbe34a9b014`  
		Last Modified: Thu, 22 Oct 2020 23:43:59 GMT  
		Size: 12.5 MB (12494146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6f70e06b6dc89317aaec50adfd52d8f2ee7f88fe47fcbf68a5adec7c98fdad`  
		Last Modified: Thu, 22 Oct 2020 23:43:51 GMT  
		Size: 7.2 KB (7158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d353780080303b0aaa6521d28febb7c2c906191e6a2a6ddee9b381d5298a6c4e`  
		Last Modified: Thu, 22 Oct 2020 23:43:51 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68c44ecf52e8a38cedb46f2db89186752750dca720c5aa2cfa5951a8578cc81`  
		Last Modified: Thu, 22 Oct 2020 23:43:50 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cf1ed629be8e282f7a83ad8c9be39033c366b806180dc40ce47368d50b1b21`  
		Last Modified: Thu, 22 Oct 2020 23:43:51 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ff792e55d1b8e76fb093b3f0c59408466b080ca2e637bd47c9e8e1c4c7a984`  
		Last Modified: Thu, 22 Oct 2020 23:43:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-alpine` - linux; s390x

```console
$ docker pull postgres@sha256:043bc5a0988b5d70581f6eaf28fb4179d09924b943833a41e599e99de93d1e8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13947828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1c0a66df00471b6b7de7c17c3de326a3ebb3154f1a837ea476d1bae51d1d082`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:05:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:05:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:05:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:23:07 GMT
ENV PG_MAJOR=9.6
# Thu, 22 Oct 2020 09:23:08 GMT
ENV PG_VERSION=9.6.19
# Thu, 22 Oct 2020 09:23:09 GMT
ENV PG_SHA256=61f93a94ccddbe0b2d1afaf03f04ba605d8af5b774ff9b830e5adeb50ab55cb0
# Thu, 22 Oct 2020 09:25:37 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:25:41 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:25:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:25:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:25:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:25:45 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:25:45 GMT
COPY file:be0996fe6c3fcec9976408f3f94ed203fdcb751cfa2cd940a2bfcbbbda925e9c in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:25:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Oct 2020 09:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:25:48 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:25:49 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:25:50 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788b366e4c5d5f3b69b31ae06b2811fe54eb39bd4fd8b6107985f9982ab150a`  
		Last Modified: Thu, 22 Oct 2020 09:29:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eed686015d5efd53e62cc5b3f61833711a48184edf03c7d21f021b34f23095`  
		Last Modified: Thu, 22 Oct 2020 09:29:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2502469121171c05fc2f76e2ad25767cecbc16ec44c84033ab905b36752eb0d`  
		Last Modified: Thu, 22 Oct 2020 09:30:42 GMT  
		Size: 11.4 MB (11368676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cc3be8653ac381149a46e7f166fde6a9ca653af9910e5f3d5a35264a36f29a`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 7.2 KB (7156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b285cd8c68c9ee9e6f882198a1940aa45563fe88a8146469b79631151b7efbf`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502a91a7c371d7662208ddf836152fadf3edeff45575861591c96ca9f5208a8b`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368653c8a2e4b08c6667d3e0a3655086f876d2b4ff5010959422ab2abfb4309`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e262a0e2bb6bc8b64f64f8fe85e555c43914c92b037beb969cb3bd3117995696`  
		Last Modified: Thu, 22 Oct 2020 09:30:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:alpine`

```console
$ docker pull postgres@sha256:d26ddee3648a324a9747b3257236322141920d5f9a82ca703def6bff1cca7067
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
$ docker pull postgres@sha256:28305dfe369277a8eaf90486c19c5d892653b914eac13b3b8b88521058b2e903
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (62014089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700e581c202ecba5ce3ffe5908a9776163a4949d289caa8319245ca9cfc6b832`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:55:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 07:55:14 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 07:55:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 07:55:15 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 07:55:15 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 07:55:15 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 08:00:51 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:00:52 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:00:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:00:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:00:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:00:54 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:00:54 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:00:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:00:54 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:00:54 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:00:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f1d1b70e7fa650fd6229086120f763219adce9e33e8b20bdfbf8452ab69847`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4f01476d2b86761cdb0414c4a583b89af3b5d0b67022cfc0d378743307f7e3`  
		Last Modified: Thu, 22 Oct 2020 08:21:53 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16419214bc023bd78d6b9098a87072ef74c349622f7320d0c84b6f326fd8b3e6`  
		Last Modified: Thu, 22 Oct 2020 08:22:00 GMT  
		Size: 59.2 MB (59202778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4886fc567835ca23c2e896a575abd09db4d3db62f1df7221bf053f624a8931cd`  
		Last Modified: Thu, 22 Oct 2020 08:21:51 GMT  
		Size: 8.5 KB (8534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9026d4fbeafa49378c5217a9f58a95633d2fcc3ea787a432d94fdbc3071e8a2c`  
		Last Modified: Thu, 22 Oct 2020 08:21:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001c336294ebcf88942d1d10c0387a319b47e9a799cea995ba87eac8c6c7760d`  
		Last Modified: Thu, 22 Oct 2020 08:21:51 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abc6d154e9fb24a05c2186f1caa1d911119a82c4b2510186de584efc34dd40b`  
		Last Modified: Thu, 22 Oct 2020 08:21:51 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v6

```console
$ docker pull postgres@sha256:9aa3390ad0b1f9eddc310269664accd38f81fa23cc91ae93d8cde6f06fb6bdf6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60195390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d24267bdc9a6b2208fc593a7eec2b1f769c57ab6946d77ecbe82b555ce85a279`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:55:00 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:55:00 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:55:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:55:03 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 08:55:03 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 08:55:04 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 08:59:31 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:59:35 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:59:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:59:39 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:59:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:59:42 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:59:43 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:59:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:59:46 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:59:48 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:59:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54bc8a79538fa79db3e734327f2a73654bc80285dc55b7e4d8d206161ec79a9`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30574d1822b9e42c2a6da5e4a8f52ab65d88be941e497b4565382967ebd326f8`  
		Last Modified: Thu, 22 Oct 2020 09:19:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1745f68cca415c7401eeaea782a52b2a9dd04a3da1e4f3ce0a4c41a4c6fa74f7`  
		Last Modified: Thu, 22 Oct 2020 09:19:36 GMT  
		Size: 57.6 MB (57578893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137f32c2f9bfab96f1336bd6d701e161f61294427613777bf68e9675475ccb20`  
		Last Modified: Thu, 22 Oct 2020 09:19:17 GMT  
		Size: 8.5 KB (8542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2099ca9f5b36ba12428c29dcff2f9ff5e1561067c9c539f3cf2f10403b73918d`  
		Last Modified: Thu, 22 Oct 2020 09:19:17 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1490f1ec1eeec24777384af72b9b5b4c3952bb6d590e30463397dd923151358b`  
		Last Modified: Thu, 22 Oct 2020 09:19:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af12193f12354e79945caf7850ac8fcd582ab67847fcca23df0046eb75dcfb8`  
		Last Modified: Thu, 22 Oct 2020 09:19:17 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm variant v7

```console
$ docker pull postgres@sha256:36ed8010aa7cb12ba66b1e4db0b8085fe08a61fc4f20b14c9dc5cf48f49fe391
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57304236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d095d11ad7acb1affe24fc9e4de91bbd54cb60004fd5315f80de26809f170dc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:56:01 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:56:03 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:56:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:56:06 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 08:56:08 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 08:56:10 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 08:59:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:59:43 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:59:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:59:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:59:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:59:51 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:59:52 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:59:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:59:53 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:59:54 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:59:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7eedf40b1ca3ca0c12781ef9399626d49e7898eb4dc6bf3888a3add86c9ee2`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2cc4a27e16f2350721162545664e1c967b92e8a0ecffb90828c979f0bc3ac6`  
		Last Modified: Thu, 22 Oct 2020 09:17:08 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9e1fc344fdc1be9247f34eb1533fd8a223cbab00b5bf4aa7459424df790ea4`  
		Last Modified: Thu, 22 Oct 2020 09:17:22 GMT  
		Size: 54.9 MB (54883977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65080db56689834b20ad68241bde5ccfa334bf0c2f80db744db6186238d2c89d`  
		Last Modified: Thu, 22 Oct 2020 09:17:06 GMT  
		Size: 8.5 KB (8540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3d3a7196b2ada5397485bfe080afd7d743d37f68d526f285b6a57887087e78`  
		Last Modified: Thu, 22 Oct 2020 09:17:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba4958fec54abe667c1f75d7c7f24dd84d87711ae546e91a16344740aeab57b`  
		Last Modified: Thu, 22 Oct 2020 09:17:06 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0fabe1fbf3b332a3379ec29ec509a3f837c46f5aac0601b8ee836c80fb9029`  
		Last Modified: Thu, 22 Oct 2020 09:17:06 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:b6399aef923e0529a4f2a5874e8860d29cef3726ab7079883f3368aaa2a9f29c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61557698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b98a8adac19738d6d88e76787142368522635722706e167bdfb7e3756f615b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:21:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 08:21:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 08:21:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 08:21:52 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 08:21:52 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 08:21:53 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 08:25:12 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 08:25:19 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 08:25:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 08:25:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 08:25:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 08:25:32 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 08:25:33 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:25:35 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 08:25:37 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 08:25:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46b3b77440641e62ecc741cdb44f0f558d15c3f3b6d506be26f8c285f7a36ff`  
		Last Modified: Thu, 22 Oct 2020 08:44:00 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85615d5b5e22de086f665265885eae6f4cb41a63e5ed6910df6d0d03d0e90c5`  
		Last Modified: Thu, 22 Oct 2020 08:43:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3399ca8ba311608fce7edea2b4b7c56e3a15651820560e526d7e892a45d9a694`  
		Last Modified: Thu, 22 Oct 2020 08:44:11 GMT  
		Size: 58.8 MB (58836563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37765dcba1abe0ee860486e0de0391cb6816ed272cea1886bc75908efac1cf77`  
		Last Modified: Thu, 22 Oct 2020 08:43:58 GMT  
		Size: 8.5 KB (8539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2093493e16e25a2e3387389fa691fab3e9a5815dd691af0c7b6f055110d738f`  
		Last Modified: Thu, 22 Oct 2020 08:43:58 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e2815f4ac9a0a90fcaf51162bacb8adcd984d8958d89c016d82c79d5291fb3`  
		Last Modified: Thu, 22 Oct 2020 08:43:58 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df26ccc1cae9303c03384992f898557df12827808b6800a3ac24718d80dbc9`  
		Last Modified: Thu, 22 Oct 2020 08:43:58 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; 386

```console
$ docker pull postgres@sha256:1dfcbfea3e85ad81b7baef84a68c8d8f8676a6b400d1ff0790929bfe1bd6d9df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65604483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201098a3f6fa14cb91820bdfbfd34469df38d7dafe93450159291da47be86f3d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:38:39 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:38:39 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:38:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:38:40 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 09:38:40 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 09:38:41 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 09:47:21 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:47:22 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:47:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:47:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:47:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:47:25 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:47:25 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:47:25 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:47:26 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:47:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596122efb908f979efd1794c09ae9c7a15ac0e4d53f2c181fd646d9f32565d9a`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeb7bd791d51cd161cadd22b53bd066e70998ebd55dd5ba92760d35f1ab9e8b`  
		Last Modified: Thu, 22 Oct 2020 10:20:51 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56896d944158831966b1797385c95616538974e5cd57e33ee6bd394de35b5b8e`  
		Last Modified: Thu, 22 Oct 2020 10:21:05 GMT  
		Size: 62.8 MB (62798615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6950449e6370c7a2e01599167c24c286b62f137d8ba017ccfd7650de7b5ba81a`  
		Last Modified: Thu, 22 Oct 2020 10:20:49 GMT  
		Size: 8.5 KB (8540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f993f62e6dccbb32c783ca06e482ddeba6cb723691026cde0c4fd16a81680558`  
		Last Modified: Thu, 22 Oct 2020 10:20:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15f2b5e39d9584dfb53e36f59b5c9d94c757d9307ee3cdce7ce4ff0a6b43414`  
		Last Modified: Thu, 22 Oct 2020 10:20:49 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51377623be83e9b7af021a2b97dde5a2e68d0a43c1ad5405d32ad212a1c717de`  
		Last Modified: Thu, 22 Oct 2020 10:20:50 GMT  
		Size: 4.3 KB (4263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; ppc64le

```console
$ docker pull postgres@sha256:10d3658d045ccb6cf6e82b372cc302bdefbadd38713b567e2980d74217492efa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64406140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897a372ceb92ff324466d266bad1e31208f1441ea3284ec9e803f0f6f1bb6649`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 23:06:14 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 23:06:17 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 23:06:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 23:06:26 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 23:06:29 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 23:06:32 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 23:10:40 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 23:10:52 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 23:11:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 23:11:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 23:11:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 23:11:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 23:11:25 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 23:11:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 23:11:33 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 23:11:40 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 23:11:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40cba28bb2e7e5449306ade2eb73dd95379370b59f2eac45aa9f62aa4d376b1`  
		Last Modified: Thu, 22 Oct 2020 23:41:44 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b145001d871735701a01931a308a05fafba12a34115cac00163359d3ed8cf19`  
		Last Modified: Thu, 22 Oct 2020 23:41:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d44cb7df0f4a70bbb8da1179c1ea586f8471e5720d0de26a1320d99ecfee94`  
		Last Modified: Thu, 22 Oct 2020 23:41:56 GMT  
		Size: 61.6 MB (61588341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0b9784976dc58199c67ea1dfa2df4d68566c102d7d1c6070322634c7ebfb6`  
		Last Modified: Thu, 22 Oct 2020 23:41:40 GMT  
		Size: 8.5 KB (8539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a35e1a562102237feab8796d8e9c6f6866dfadf1efc57d1b329b2d221d66d88`  
		Last Modified: Thu, 22 Oct 2020 23:41:41 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4facb5bf19a8bb8f97f75e520566074ccae805f4b863d6e48d699c4b204908b`  
		Last Modified: Thu, 22 Oct 2020 23:41:40 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8082c85c7c0de55885ba799e76111f5e1b288bef480873b2cecd123bd1af223`  
		Last Modified: Thu, 22 Oct 2020 23:41:41 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:alpine` - linux; s390x

```console
$ docker pull postgres@sha256:e5a1e46e00aac62a7a70a4ee5811850b00267b3eabbe0c36bfb173014b996930
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.5 MB (64479911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeac1e50499ae7b21de2a4952e8bd9bc474c80b6e400748dcc3390fab7f07afa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 09:05:49 GMT
RUN set -eux; 	addgroup -g 70 -S postgres; 	adduser -u 70 -S -D -G postgres -H -h /var/lib/postgresql -s /bin/sh postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 22 Oct 2020 09:05:49 GMT
ENV LANG=en_US.utf8
# Thu, 22 Oct 2020 09:05:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 22 Oct 2020 09:05:51 GMT
ENV PG_MAJOR=13
# Thu, 22 Oct 2020 09:05:51 GMT
ENV PG_VERSION=13.0
# Thu, 22 Oct 2020 09:05:52 GMT
ENV PG_SHA256=80e750be8d436b54197636a02636f8fd3263ba6779bf865b04832495ea592296
# Thu, 22 Oct 2020 09:10:07 GMT
RUN set -eux; 		wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2"; 	echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c -; 	mkdir -p /usr/src/postgresql; 	tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	; 	rm postgresql.tar.bz2; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		llvm10-dev clang g++ 		make 		openssl-dev 		perl-utils 		perl-ipc-run 		util-linux-dev 		zlib-dev 		icu-dev 	; 		cd /usr/src/postgresql; 	awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new; 	grep '/var/run/postgresql' src/include/pg_config_manual.h.new; 	mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb'; 	wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb'; 	./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 		--with-icu 		--with-llvm 	; 	make -j "$(nproc)" world; 	make install-world; 	make -C contrib install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	; 	apk del --no-network .build-deps; 	cd /; 	rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	; 		postgres --version
# Thu, 22 Oct 2020 09:10:15 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Thu, 22 Oct 2020 09:10:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 22 Oct 2020 09:10:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 22 Oct 2020 09:10:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 22 Oct 2020 09:10:19 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 22 Oct 2020 09:10:20 GMT
COPY file:8f542efd076b9b67ef64928f3c0185ed50bfcbbc3572436a7222e879810d747f in /usr/local/bin/ 
# Thu, 22 Oct 2020 09:10:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 09:10:21 GMT
STOPSIGNAL SIGINT
# Thu, 22 Oct 2020 09:10:21 GMT
EXPOSE 5432
# Thu, 22 Oct 2020 09:10:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788b366e4c5d5f3b69b31ae06b2811fe54eb39bd4fd8b6107985f9982ab150a`  
		Last Modified: Thu, 22 Oct 2020 09:29:06 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eed686015d5efd53e62cc5b3f61833711a48184edf03c7d21f021b34f23095`  
		Last Modified: Thu, 22 Oct 2020 09:29:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b5c49866375be63b5c0df20d45eff9b155100b10e2dad36b6369fa8dcb1e2d`  
		Last Modified: Thu, 22 Oct 2020 09:29:13 GMT  
		Size: 61.9 MB (61899505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b283091e8db48015a3a673e2074af8a40665adc59da43ae21251bc54e3fcd8`  
		Last Modified: Thu, 22 Oct 2020 09:29:04 GMT  
		Size: 8.5 KB (8535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb452e6ac31ed779bdb65f15850af5b72bc90c8a4031dd945a1c2a3adb16a75`  
		Last Modified: Thu, 22 Oct 2020 09:29:04 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc54b509173838bf179855e6124b92bc8f5d7f55809b0956165e22290c5d5c3`  
		Last Modified: Thu, 22 Oct 2020 09:29:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab84a2f6ff3bdde6b5575c71c358f3642d9fa6ad4b91ccdcce2fe3d43dc2bd6`  
		Last Modified: Thu, 22 Oct 2020 09:29:04 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `postgres:latest`

```console
$ docker pull postgres@sha256:8f7c3c9b61d82a4a021da5d9618faf056633e089302a726d619fa467c73609e4
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
$ docker pull postgres@sha256:832e01fa055c55a9c9195db231cf3935a81b7b60c8cccd64e7b5395d1ee1948b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114727939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c96f8b6bc0d9f0277f118cf485a8c302e32cfe05e7d65f6e9a4c106679439d5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:31:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:31:49 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:31:49 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:31:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:32:06 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:32:07 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:32:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:32:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:32:13 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:32:14 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 12:32:14 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 12:32:34 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:32:35 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:32:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:32:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 12:32:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:32:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:32:37 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:32:37 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:32:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:32:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:32:38 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:32:39 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:32:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dc51fa2b560b7daf34aa4c2501941b4ce0d701c4ecf571777b13d79561f1bc`  
		Last Modified: Tue, 13 Oct 2020 12:37:32 GMT  
		Size: 4.2 MB (4178093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f213b6f96d81fa40e97b4eb61a159f716d77a4c70a25f376525385d7836bdee2`  
		Last Modified: Tue, 13 Oct 2020 12:37:31 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2780ac832fdea1b95491eaf082507289c13fc77e97de2716ee80e851cce0c79a`  
		Last Modified: Tue, 13 Oct 2020 12:37:31 GMT  
		Size: 1.4 MB (1419193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5cee1a3f123d23889bfdd0941b304d3906c90e136ec0e13f340b473096902f`  
		Last Modified: Tue, 13 Oct 2020 12:37:33 GMT  
		Size: 8.0 MB (7964517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95db3c06319e21f4c21eff545348f1755e5979d63c551a5b82bf9ff55ef30fa5`  
		Last Modified: Tue, 13 Oct 2020 12:37:30 GMT  
		Size: 391.1 KB (391050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475ca72764d52e2efe3b99160dbf36815c6be1ffda0790cc7e22354796185f08`  
		Last Modified: Tue, 13 Oct 2020 12:37:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d602872ecaeaf9c80cc4728578cc9a9b42d53b5f9351195a60f0be4455f99fd`  
		Last Modified: Tue, 13 Oct 2020 12:37:30 GMT  
		Size: 3.1 KB (3053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fca31f2e3d83c36758a751e320fd26cb77d6f17a5f07b73989d935ddbfd510`  
		Last Modified: Tue, 13 Oct 2020 12:37:46 GMT  
		Size: 73.7 MB (73663978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00c442835e0871a8bcee1d389c603ff88190004b04ab5186d59836f2c3379e8`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 9.3 KB (9266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2305af339024dfd3d40697adb93e5ccb8decba5337e3eef1979ee4a2f151ca`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cff852bb872a5b4dd86f2528157acb8c3ab2f59f5bce84a91e38990afb7e798`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bb0be115435b86fab9f9ac77ee9b01ca697d631038ff6e062ff203baf0a1fb`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 4.3 KB (4257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4738c099c4ad0480a6ea8a835aaf6777de42ec140984844cd53b9e05f8c44004`  
		Last Modified: Tue, 13 Oct 2020 12:37:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v5

```console
$ docker pull postgres@sha256:38603a6ed6b60e32bd2c3358ae627f1d1abf2213c4b9a480895d6ca55c2b99a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.9 MB (108938865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfd776c8231424dc528ba84f657cb51287071d6b6b792d2b328fe4e13f5c51a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 06:16:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 06:16:12 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 06:16:13 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 06:16:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 06:16:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 06:16:48 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 06:16:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 06:17:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 06:17:03 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 06:17:04 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 06:17:05 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 06:43:30 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 06:43:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 06:43:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 06:43:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 06:43:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 06:43:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 06:43:42 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 06:43:42 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 06:43:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 06:43:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 06:43:47 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 06:43:48 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 06:43:49 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220f749165a848f7f38bac836c52f4b835c99e7d95e05ee20dadaec192039226`  
		Last Modified: Tue, 13 Oct 2020 08:36:06 GMT  
		Size: 3.8 MB (3847907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99328c93a7de72d797aa8f54b8f5f65ac8dcfcb8adfcf619deb383521090b6a8`  
		Last Modified: Tue, 13 Oct 2020 08:36:05 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877588e4293d5c0bc10377dd6a2128f747be69e1e9176d0d8a2e6408917422ff`  
		Last Modified: Tue, 13 Oct 2020 08:36:05 GMT  
		Size: 1.4 MB (1378519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa96f5e00aa670ea297c3d7b88aef48e3e83cecb4a2957ba6e1193fc4f3a0eba`  
		Last Modified: Tue, 13 Oct 2020 08:36:06 GMT  
		Size: 8.0 MB (7965207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e8a16e6b99574961ad43e457e425366fa1f111b3ce41c801ae3c66b5e68c86`  
		Last Modified: Tue, 13 Oct 2020 08:36:03 GMT  
		Size: 390.4 KB (390390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511e0945d4fb63b1f0366268b49f03e65681c8615d784c5ba2485563cf6d1f21`  
		Last Modified: Tue, 13 Oct 2020 08:36:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834364422035b3d7732f4346f19965cb41e38c4e33423185259f014337b1cfa0`  
		Last Modified: Tue, 13 Oct 2020 08:36:03 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf7b596aa05f83df06a644f9ce328ce279a1e0ba14b85696788de96ab737ddb`  
		Last Modified: Tue, 13 Oct 2020 08:36:25 GMT  
		Size: 70.5 MB (70501869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb22e708f1b3e5dff44453d0399222d13620e8be2f2c772c8d456c856f96da4`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 9.3 KB (9271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4403bcf196b9551826b50231481ba507bb6af5296da7e058aa8ca275bec41a2d`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa44359c6208940bde933378068055f585c04b80ccc76ec3d893142a68effd8d`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f819a8254858e6516d31a74081043ed355681e338f5849486a307a2aa19048e`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28de01a1ab0d2e4e95474888fc65ad4af854f91efa1f14f065382069ebc0917e`  
		Last Modified: Tue, 13 Oct 2020 08:36:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v7

```console
$ docker pull postgres@sha256:9065c211f3d3b9f1f636403fcaa495416e6f3d1f194ffb957ab7ebf2119b4508
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104973664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28765e01da329697bcf5759441aad1e5e1ced29720adde286516666a1f31b0dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:03:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:03:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:03:10 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:03:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:03:51 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:03:52 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:04:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:04:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 05:04:10 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 05:04:11 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 05:29:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 05:29:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 05:29:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 05:29:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 05:29:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 05:29:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 05:29:16 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 05:29:17 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:29:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 05:29:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 05:29:21 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 05:29:21 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 05:29:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9abeb7fdbbade7b8abd012862e54cc393b34cd5ded22d30651c3d96f804017`  
		Last Modified: Tue, 13 Oct 2020 07:07:55 GMT  
		Size: 3.5 MB (3481628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c060aae45342f7e836211d989e2a8acbbc00aa77c9cedf463bc22d3931011b38`  
		Last Modified: Tue, 13 Oct 2020 07:07:54 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df78177be2b9c4f60b1d775bbe3774b00e3c1c567c4f122bbdff0d8c9be841a8`  
		Last Modified: Tue, 13 Oct 2020 07:07:54 GMT  
		Size: 1.4 MB (1370276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb71a60beb691d7f1f8351012f0a88049401c5ee2057e4a830758eee6c8dae4`  
		Last Modified: Tue, 13 Oct 2020 07:07:55 GMT  
		Size: 8.0 MB (7965243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d3d3aab018a14d7c2ecdf71b6ba41d4a5521ba93a7a91a5ef2c466512f6165`  
		Last Modified: Tue, 13 Oct 2020 07:07:52 GMT  
		Size: 385.0 KB (385046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2443ca999a57081e3059a2ce066d226d974c0bfe22f8f887df06da48744d1b04`  
		Last Modified: Tue, 13 Oct 2020 07:07:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f35f400211e43d2986188ba441aee4ef58990df42a4f6215d473f4162cc97b5`  
		Last Modified: Tue, 13 Oct 2020 07:07:51 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7812530b8edbe3e8038a3f3ec17ae95fd1589ae6341af1725858e1d0b02394`  
		Last Modified: Tue, 13 Oct 2020 07:08:13 GMT  
		Size: 69.1 MB (69052639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f22889ebf9de2c6d34abee77286c2e5ff8184fd3b9e97d8a0ec4ff9303219fb`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 9.3 KB (9273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc99b88e591c236507bc93a29ac74921a6a9c6e09472065b67665870ed09f19`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a4c25625ec9a36c08c757ef59b112d266f6cef4d71a069746026f925ee9796`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eb3b82d2dfbb399ffeaff5992b19368614746e01205a39973031aa9bf667dc`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7031c8ae6bfe4c28598680fbfab04adb945f369033071a41102ccf52d070c6`  
		Last Modified: Tue, 13 Oct 2020 07:07:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:0f96f9bd3099ebac30627729927a4be150465a669c0e79cf2fc94fda8c4f1248
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111040907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56731e2258858f1bf427e3050f388dc3e80d42b6077e433931c70fa32065a096`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:01:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 11:01:16 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 11:01:17 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 11:01:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 11:01:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 11:01:49 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 11:01:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 11:02:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 11:02:04 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 11:02:05 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 11:02:06 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 11:02:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 11:02:43 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 11:02:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 11:02:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 11:02:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 11:02:47 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 11:02:48 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 11:02:48 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 11:02:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 11:02:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 11:02:51 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 11:02:52 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 11:02:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b54dce2ac1eb5c484547daceb63d77b4ebf86f7adfd08524a95ce1aff995a0`  
		Last Modified: Tue, 13 Oct 2020 12:19:50 GMT  
		Size: 4.2 MB (4170140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35640a43c389c81984759b8bf006675c2a1e3022a8d2d264a668d146e4769dbd`  
		Last Modified: Tue, 13 Oct 2020 12:19:47 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954d8cf15b37983553c28d10814bd8446e8868be10ddf07020e44a34f42f42b0`  
		Last Modified: Tue, 13 Oct 2020 12:19:48 GMT  
		Size: 1.4 MB (1354215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cabadd29423fceb4b9404f0cd2f1acbbd9e1a5ae16cb2ede30fb5d61c03754d`  
		Last Modified: Tue, 13 Oct 2020 12:19:50 GMT  
		Size: 8.0 MB (7965226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1dd2db3831e8b25aa548ca0e46c9d5401d403008baebac964b6d92481f854b`  
		Last Modified: Tue, 13 Oct 2020 12:19:47 GMT  
		Size: 389.5 KB (389459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4df45b4efe24423097c32f0333b82820205f47b219e75a9ef9cb82de56f0b5`  
		Last Modified: Tue, 13 Oct 2020 12:19:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c896ba7aabec2bed17223fe6f2f53f9d77908d0d1103da3be9285dd1916e12dd`  
		Last Modified: Tue, 13 Oct 2020 12:19:46 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598355fbe9f5b6cd68053bc6fe6357bb74394c1a74d2b8246e3fa01f4dddb68c`  
		Last Modified: Tue, 13 Oct 2020 12:20:05 GMT  
		Size: 71.3 MB (71293545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc69a8470043117cb274d54203477ac732c8cc100ce015512f6bcb3b24df6b9`  
		Last Modified: Tue, 13 Oct 2020 12:19:41 GMT  
		Size: 9.3 KB (9270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3bea9860ee50eb0f0f3090fc98b246f3f1ff8797f292526285de1c6e77b573c`  
		Last Modified: Tue, 13 Oct 2020 12:19:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d44ba2b6c2bafc61dac4cb65a9a6da79a2eb11bce12324ae132d4cde3e631a8`  
		Last Modified: Tue, 13 Oct 2020 12:19:43 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1f22e595f6fdf38d7d04949e2ff149b9d62f547aa1cb0ec7c262af3bfe5f10`  
		Last Modified: Tue, 13 Oct 2020 12:19:41 GMT  
		Size: 4.3 KB (4257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f34ec236671db6a5b58d63a24446815ee2e0468f8826bba296f23dea12fd644`  
		Last Modified: Tue, 13 Oct 2020 12:19:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; 386

```console
$ docker pull postgres@sha256:f018e9368b20e43b78fdb2913ac69058b0c1e97acee248d6b00765609237d6f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115393152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396efc10231f414e89419a0156bda225c11bb0060c11071bf85eebec57418980`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 16:41:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 16:41:02 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 16:41:02 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 16:41:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 16:41:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 16:41:23 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 16:41:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:41:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 16:41:30 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 16:41:30 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 16:41:30 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 16:41:56 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 16:41:57 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 16:41:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 16:41:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 16:41:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 16:41:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 16:41:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 16:41:59 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 16:42:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 16:42:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 16:42:01 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 16:42:01 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 16:42:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c749690104cd2d067ab453dc94a6cb768cf70e8de2c7b070e3ec6c77cbea76`  
		Last Modified: Tue, 13 Oct 2020 16:47:28 GMT  
		Size: 4.5 MB (4542310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53e540fa0f9a8216d1625184511d7ae088dfb209a6bfbb7b01c9c28c386c29b`  
		Last Modified: Tue, 13 Oct 2020 16:47:25 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f01c54b9c4b48006dab4a6cb134885abb354aeded9eacda10b26e602331d0cb`  
		Last Modified: Tue, 13 Oct 2020 16:47:26 GMT  
		Size: 1.4 MB (1389505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabc4d4ec793f5e333d10d49bbf35728a1ddc5fa3b6e52c352e3d895ac7e082d`  
		Last Modified: Tue, 13 Oct 2020 16:47:31 GMT  
		Size: 8.0 MB (7964471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375c7950de1c2fb505ecd4b84309dceec40018957c961d9cea659485543b3d02`  
		Last Modified: Tue, 13 Oct 2020 16:47:24 GMT  
		Size: 398.2 KB (398247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bdf70f6f30cc05214496056e156b19a2a2e44644781822d902a04d7011b734`  
		Last Modified: Tue, 13 Oct 2020 16:47:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edb30201e63d9b68cdbed38ee43fd90089112ea5608240ebd879220b62db189`  
		Last Modified: Tue, 13 Oct 2020 16:47:23 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191d0c377d25905e6dcc7b0de1ec1f2a925efa054feeaa7c4f346f5e646909a7`  
		Last Modified: Tue, 13 Oct 2020 16:47:55 GMT  
		Size: 73.3 MB (73329502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55cc6354a2dd5815e1a906ddf70063dc921507ad77e83ff37dae5169aa089eb`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 9.3 KB (9267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c77e86a23757931392202f1860011dca42b38ce451321f063b5173e3eb8d1f7`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0968e8f318a7dfc521a4a9dc8a9f35b5c096513aacaeda21888f91910aabf8`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af57a264872aebf23e30761bdd8f746d80cdde00ab2b6aca8f8becb55339782d`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dec4d85f466ca05a9c86992e601e395a740f8a0d8cf148f7bd57921a97818c`  
		Last Modified: Tue, 13 Oct 2020 16:47:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; mips64le

```console
$ docker pull postgres@sha256:6cdacd4e1e6463e0e88873d0293840c2db7fae74843994071b1e0995545574e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110310541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6c25d52c34151663ac0addf97fb0c57175829ccd2d35b3e80aea8d5728ffda6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:13:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 13:13:38 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 13:13:38 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 13:13:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 13:14:23 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 13:14:24 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 13:14:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 13:14:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 13:14:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 13:14:41 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 13:14:41 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 14:06:36 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 14:06:39 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 14:06:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 14:06:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 14:06:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 14:06:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 14:06:44 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 14:06:44 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 14:06:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 14:06:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 14:06:47 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 14:06:47 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 14:06:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e607f4b85ab0160062c5b0997b24f9c552c3b0a99c818918df616f061bc1582`  
		Last Modified: Tue, 13 Oct 2020 14:57:06 GMT  
		Size: 4.2 MB (4182331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2e3c1d8252ef141fbeb05954df9c4cffe4be8a378178b0f7bc970a74a6c7a5`  
		Last Modified: Tue, 13 Oct 2020 14:57:02 GMT  
		Size: 1.8 KB (1774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea3f4e38a84676f0d0f445a051330b19231188038d657dd3578c9ca400f1984`  
		Last Modified: Tue, 13 Oct 2020 14:57:03 GMT  
		Size: 1.3 MB (1307194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bc9170e37b7197108bb722eaee5a99c4b901d9be26a821a6b1d4db05f4362`  
		Last Modified: Tue, 13 Oct 2020 14:57:07 GMT  
		Size: 8.0 MB (7964635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab188a504bfa78fc88e311060cec8f95d3e3117d1419d605ac3ff070b82d000`  
		Last Modified: Tue, 13 Oct 2020 14:56:59 GMT  
		Size: 389.2 KB (389250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94c8867122219de48b09839756b0ffd313a762e792727c7390ae175987591ab`  
		Last Modified: Tue, 13 Oct 2020 14:56:59 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079c91791bcc494ca3ceef784e9686b641a2dfd712ce9279a1b3f406a9c2dce0`  
		Last Modified: Tue, 13 Oct 2020 14:56:59 GMT  
		Size: 3.1 KB (3060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ed439ff0db80133ad5c64fd6f680da2629710df67c477195efe628627f8aa9`  
		Last Modified: Tue, 13 Oct 2020 14:57:49 GMT  
		Size: 70.7 MB (70685659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ef9de52f6e2ba62c847999fa0535d0640c61757dbce18666ef659edd3a715c`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 9.3 KB (9271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1306e8acbffe7d13f0aff7b96ee72fb777ff29690469d9a9c6abcdb37686be56`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102f301ca71ccd15c8150f9420fe86cb7f59885a1f4d0742fc76d7cff131dc4`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e563574ec7e322fff2134f1556e556d32d17984dd3a35fb760389b3fd08551a7`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e039d4d6237abc30a0d5f84382970f19bd8bd887db7069953d0c3a122ce3ad`  
		Last Modified: Tue, 13 Oct 2020 14:56:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; ppc64le

```console
$ docker pull postgres@sha256:cb47cd3347f142ab699462939df23ed7ab245a76ecca75c6c7143e1707c5694c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122023914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8032178de335da47dffe309bcfdb072cbed6334b8d2a45717a1b891963c3d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:31:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 12:31:39 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 12:31:42 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 12:32:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 12:33:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 12:33:13 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 12:33:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:34:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 12:34:16 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 12:34:20 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 12:34:24 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 12:35:57 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 12:36:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 12:36:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 12:36:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 12:36:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 12:36:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 12:36:43 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 12:36:44 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 12:36:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 12:37:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 12:37:03 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 12:37:07 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 12:37:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561d545502ace2058d00663781db14dfa7756b6edb0acc8d79700400b867d9`  
		Last Modified: Tue, 13 Oct 2020 12:42:26 GMT  
		Size: 5.0 MB (4967255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ce5eebcabcdc9f2911ca87a8ab93cf539c873fa6cd96595dd928263e616b0`  
		Last Modified: Tue, 13 Oct 2020 12:42:22 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623858b6704dcb200beeee22ceb00bbeed4613a5b3d2df4ea7e457712e441d52`  
		Last Modified: Tue, 13 Oct 2020 12:42:22 GMT  
		Size: 1.3 MB (1337966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740971b5e3abf8f64361a1c8b2c4925b1c6f6a64ff7bd7482fa567278cd16ad6`  
		Last Modified: Tue, 13 Oct 2020 12:42:17 GMT  
		Size: 8.0 MB (7965414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8928d4fa7be49ec051fe27e367a44509f36af44275dabf2115d9dadadda84`  
		Last Modified: Tue, 13 Oct 2020 12:42:14 GMT  
		Size: 397.0 KB (397010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa177700b6800c9f06584f40ca975a9845416cfda21bc3e479c67addaf7aed1e`  
		Last Modified: Tue, 13 Oct 2020 12:42:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91522516c8e69fabb5c9cbbb1e69764d59bc27dfba6a6a86c1f1d334abdea069`  
		Last Modified: Tue, 13 Oct 2020 12:42:14 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420d0a7efbf19ebce8f0088536a373b3205d7466526a64b3dae9f5423362edc0`  
		Last Modified: Tue, 13 Oct 2020 12:42:29 GMT  
		Size: 76.8 MB (76819402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32c8c22f6099516385dade75212072689a00ecaa4e2034386050b6b785c8529`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 9.3 KB (9268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92629bd5781650a7387e7af4a085d350ab77b488099d6e82ce955f2f03ffe57d`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7347194451e408bb9299f91edc3f6c9f3dce6779ed0ccf606fdb9f162b038165`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9193f231104f9dfe1bdb76f320002ba8f6730d35c8f8fa475ae27ad533682c6`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30870777ec22e86f3dba3808deb5da9b9a5427e1c804b15d21140d9c9e51424e`  
		Last Modified: Tue, 13 Oct 2020 12:42:08 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; s390x

```console
$ docker pull postgres@sha256:0aab83a6545cdd6b3814844c7b27a15e7ebc25fdb3d1d24610e73c21cc7db077
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.0 MB (113041886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50ac0b622ec547412072ab8b679c2d557f7172284518c9caf272ddb43aec4ca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:29:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 05:29:42 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 13 Oct 2020 05:29:43 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:29:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 05:30:00 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 13 Oct 2020 05:30:01 GMT
ENV LANG=en_US.utf8
# Tue, 13 Oct 2020 05:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 05:30:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 05:30:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 13 Oct 2020 05:30:07 GMT
ENV PG_MAJOR=13
# Tue, 13 Oct 2020 05:30:08 GMT
ENV PG_VERSION=13.0-1.pgdg100+1
# Tue, 13 Oct 2020 05:39:30 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Tue, 13 Oct 2020 05:39:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 13 Oct 2020 05:39:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 13 Oct 2020 05:39:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 13 Oct 2020 05:39:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 13 Oct 2020 05:39:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 13 Oct 2020 05:39:36 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 13 Oct 2020 05:39:36 GMT
COPY file:319b7406843f62370047c33da3dd702120d7eec161b31772aa6de0f02a6b3a94 in /usr/local/bin/ 
# Tue, 13 Oct 2020 05:39:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 13 Oct 2020 05:39:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 05:39:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Oct 2020 05:39:38 GMT
EXPOSE 5432
# Tue, 13 Oct 2020 05:39:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7246467ce71536a8e2ade5b913ba8c8c2c284426242907721099dceee57b3d`  
		Last Modified: Tue, 13 Oct 2020 05:47:38 GMT  
		Size: 4.1 MB (4059880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fbfd1313b673513f09c3f4ca8987bb77c156970039a431c5e677c2518b5ce7`  
		Last Modified: Tue, 13 Oct 2020 05:47:37 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316d02a9da51a3528085a50af6a3c3fc112a9892918038b44473e607269bce40`  
		Last Modified: Tue, 13 Oct 2020 05:47:37 GMT  
		Size: 1.4 MB (1406018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec69c124ec4c64206aeea60c42ea10de9b1af911bd0efc456c487758989c627`  
		Last Modified: Tue, 13 Oct 2020 05:47:36 GMT  
		Size: 8.0 MB (8019393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1b1f52aea9588cf7dfe5864c787e643d0461967d4b63ce5186c896f2c7af72`  
		Last Modified: Tue, 13 Oct 2020 05:47:34 GMT  
		Size: 388.3 KB (388335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6429d50d17c8727d414f90680190cb9ff6d4d7e439a98bcb910575ed9cbf79`  
		Last Modified: Tue, 13 Oct 2020 05:47:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5cf466603f40623a27a57ca6f4c0148a2b16cfa2beaec1b72745cb3123df5d`  
		Last Modified: Tue, 13 Oct 2020 05:47:34 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511d1c3258fd3b50e59f2508c15a8012230255ffaadb4a60b3e627e45a528d2c`  
		Last Modified: Tue, 13 Oct 2020 05:47:44 GMT  
		Size: 73.4 MB (73441752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320a06bf97139418261449c854dd4c2c5f3c62cc46a7ec5b79db8df49ef2d0`  
		Last Modified: Tue, 13 Oct 2020 05:47:32 GMT  
		Size: 9.3 KB (9271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4964cb4e537ebb6eb9840daa00c600a9fb570b5eb8a25db62f692d995d7443c`  
		Last Modified: Tue, 13 Oct 2020 05:47:33 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7a1074d81612d7507a6fe22514c36a9e5c1d65acd408b92640e10767898c85`  
		Last Modified: Tue, 13 Oct 2020 05:47:32 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305ce2b8a378c07a61cbc72936f4f9f922e7bc65147995fb54d39590fa774d8e`  
		Last Modified: Tue, 13 Oct 2020 05:47:32 GMT  
		Size: 4.3 KB (4260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d384c65ea5d63596390498b0b7ea2023e387bb9d771fbd297a40e5180fb480d5`  
		Last Modified: Tue, 13 Oct 2020 05:47:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
