## `postgres:15-bullseye`

```console
$ docker pull postgres@sha256:40c61dc2f347194e8e28614440d773f0325be7b4998d642e374223ec2d6db7f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `postgres:15-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:dcfdb5d499b04f8d0b4219b07dac07b336923a18255322c95c11d7acd7501aab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138965326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c88fbae765e8bcdb4c8974c73279e9c00b3bb5ab7e23131e40706430ef2bb2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 23 May 2023 01:20:14 GMT
ADD file:88252a7f118b4d6f55dd5baf49dbcaa053c9d6172c652963c1151fa76f625e44 in / 
# Tue, 23 May 2023 01:20:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:16:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 23 May 2023 09:16:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 09:16:59 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 09:17:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 09:17:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 23 May 2023 09:17:14 GMT
ENV LANG=en_US.utf8
# Tue, 23 May 2023 09:17:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 09:17:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 09:17:19 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 09:17:19 GMT
ENV PG_MAJOR=15
# Tue, 23 May 2023 09:17:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 23 May 2023 09:17:19 GMT
ENV PG_VERSION=15.3-1.pgdg110+1
# Tue, 23 May 2023 09:17:37 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 23 May 2023 09:17:38 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 23 May 2023 09:17:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 23 May 2023 09:17:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 23 May 2023 09:17:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 23 May 2023 09:17:39 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 23 May 2023 09:17:39 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 23 May 2023 09:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 09:17:39 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 09:17:39 GMT
EXPOSE 5432
# Tue, 23 May 2023 09:17:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f03b40093957615593f2ed142961afb6b540507e0b47e3f7626ba5e02efbbbf1`  
		Last Modified: Tue, 23 May 2023 01:24:08 GMT  
		Size: 31.4 MB (31403586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d674c93414d86da557bb0c5d586c97fd8891de2bdcf3e57f6deca4c4ee51722`  
		Last Modified: Tue, 23 May 2023 09:20:00 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de781e8e259a843f1fdb5d65faed1fb6327f4fd796c072d658cc9df8c79275df`  
		Last Modified: Tue, 23 May 2023 09:20:00 GMT  
		Size: 4.4 MB (4415031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea6efaf51f64e2a377ffe0f6fe876e7a9efe5ad666cb080ad67de4171956793`  
		Last Modified: Tue, 23 May 2023 09:19:59 GMT  
		Size: 1.5 MB (1471540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b078d5f4ac8274676d081ea230c8494ff9c7f4702e4151fde7af12c8c35a9d05`  
		Last Modified: Tue, 23 May 2023 09:19:59 GMT  
		Size: 8.0 MB (8045516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f84fb2a9182a235af20b24157f5574fa6678efc93a59e4903028cea8c8f7d2`  
		Last Modified: Tue, 23 May 2023 09:19:57 GMT  
		Size: 1.3 MB (1261285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6bf2f43fb849ae72cca21064f816c73617232c7e92ed0c2dd9518980b5cea5`  
		Last Modified: Tue, 23 May 2023 09:19:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a40e88fea491d6966f7a9c026df92f7289f38d49be29d419435388efc1e89a`  
		Last Modified: Tue, 23 May 2023 09:19:57 GMT  
		Size: 3.2 KB (3203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be673794a1a73fd5bff848268081d9d83a7c99df2bc4ddb7a9e7c0ef1735a59`  
		Last Modified: Tue, 23 May 2023 09:20:07 GMT  
		Size: 92.3 MB (92348316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d72f84fb8618038600e61f2f8b653eb0fd8ee987b8725dfa368f4e5f1f33758`  
		Last Modified: Tue, 23 May 2023 09:19:55 GMT  
		Size: 9.8 KB (9784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d52569da92e6b8ac94bda65917961654fde0d8712ffa731082abd5126a567b9`  
		Last Modified: Tue, 23 May 2023 09:19:55 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d48fbe991ff24ce4158a5a96b66762a095664705624325935d5488046a872a5`  
		Last Modified: Tue, 23 May 2023 09:19:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae692d11ad371dd258adfcc696f09db9ed56184616207e62f65494890894b42`  
		Last Modified: Tue, 23 May 2023 09:19:55 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:d46aa12411f9af93c677619c40031aaafff8db2a82e7f602bcae7c0d85f6e4af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132234582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3301203fd997051479c9919e86a600ced03d0ce76e3afa4f7c6b0c5caf85669c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 23 May 2023 00:48:41 GMT
ADD file:868f634f5ddb80ed9e9c719ccaf5d564d96fe819f0b000ecc734311baf5da99b in / 
# Tue, 23 May 2023 00:48:42 GMT
CMD ["bash"]
# Tue, 23 May 2023 06:31:24 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 23 May 2023 06:31:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:31:31 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 06:31:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 06:31:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 23 May 2023 06:31:49 GMT
ENV LANG=en_US.utf8
# Tue, 23 May 2023 06:31:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:31:55 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 06:31:56 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 06:31:57 GMT
ENV PG_MAJOR=15
# Tue, 23 May 2023 06:31:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 23 May 2023 06:31:57 GMT
ENV PG_VERSION=15.3-1.pgdg110+1
# Tue, 23 May 2023 06:46:13 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 23 May 2023 06:46:15 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 23 May 2023 06:46:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 23 May 2023 06:46:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 23 May 2023 06:46:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 23 May 2023 06:46:17 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 23 May 2023 06:46:17 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 23 May 2023 06:46:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 06:46:17 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 06:46:17 GMT
EXPOSE 5432
# Tue, 23 May 2023 06:46:17 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:812967ccba449e7a96044b2d48ffc62816b22eb17641844c4dfffbe3b3ec6f21`  
		Last Modified: Tue, 23 May 2023 00:51:19 GMT  
		Size: 28.9 MB (28903411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4491730e6ccb68eaf6ed1d8ed7ddee00a95decbd55a273a239180d7a883899`  
		Last Modified: Tue, 23 May 2023 07:39:04 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a65a1e087f29963ca9f77dde6aa85968e32fd46e04daef7c19a3ff9c8daa08`  
		Last Modified: Tue, 23 May 2023 07:39:04 GMT  
		Size: 4.1 MB (4096632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f2ead475e77a31ec431d77500d3995713cf8f6f9fae3e8df827e9f9a931436`  
		Last Modified: Tue, 23 May 2023 07:39:04 GMT  
		Size: 1.4 MB (1448825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75bcc469fe3379ffc11c94494eab66b49ac5c304787f5d9b322a9ab54597bc4`  
		Last Modified: Tue, 23 May 2023 07:39:03 GMT  
		Size: 8.0 MB (8045491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3d6533d770df470e5455ec600f7e439078dbf817756c7c1cff483484b92328`  
		Last Modified: Tue, 23 May 2023 07:39:02 GMT  
		Size: 1.3 MB (1257384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047c65f43a73cfe2d5d1d139ffe1ca0edcad7f65f9401e8c34ea2cfe55bd74a`  
		Last Modified: Tue, 23 May 2023 07:39:01 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3098f82a77bbeeb68cc3b17c6a1acdc77fca598079a410460ae852171d82c55f`  
		Last Modified: Tue, 23 May 2023 07:39:01 GMT  
		Size: 3.2 KB (3195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4cd1ddfb13425cce8448cabdf80f6be7c6f30a8573ab36adfda43ee6c203a9`  
		Last Modified: Tue, 23 May 2023 07:39:12 GMT  
		Size: 88.5 MB (88462801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58dbcef66711aba12d1e3a8d62cc8590a4f1e95149559297444ed3fb6d10170`  
		Last Modified: Tue, 23 May 2023 07:38:59 GMT  
		Size: 9.8 KB (9789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048a2cbfab6fad5f6c06feceb4fde7e10c894f32a3e658926ceb83848cf48ad2`  
		Last Modified: Tue, 23 May 2023 07:38:59 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb4cc1cfb7be2abf558389df96a354c8114392ed70e2f26bd34df2f7062eae4`  
		Last Modified: Tue, 23 May 2023 07:38:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3d335f58acfc7fa30ace3e8f6cc3500b990eac0326f3ba6e0af487fea89ad0`  
		Last Modified: Tue, 23 May 2023 07:38:59 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:310173a2633683ebb9884c7fabbff6464825cb11e2bfd64033357e83f97881d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126880813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baba3becd2695876a087cc9dc6a5f39069440280e223cc9789677bb2be9ae302`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 08:26:16 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 23 May 2023 08:26:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 08:26:28 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 08:26:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 08:26:52 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 23 May 2023 08:26:52 GMT
ENV LANG=en_US.utf8
# Tue, 23 May 2023 08:26:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 08:27:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 08:27:03 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 08:27:03 GMT
ENV PG_MAJOR=15
# Tue, 23 May 2023 08:27:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 23 May 2023 08:27:04 GMT
ENV PG_VERSION=15.3-1.pgdg110+1
# Tue, 23 May 2023 08:41:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 23 May 2023 08:41:43 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 23 May 2023 08:41:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 23 May 2023 08:41:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 23 May 2023 08:41:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 23 May 2023 08:41:44 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 23 May 2023 08:41:44 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 23 May 2023 08:41:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 08:41:44 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 08:41:44 GMT
EXPOSE 5432
# Tue, 23 May 2023 08:41:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b655d8d77c7a916b5daeaa50b58de4d419191253dd3eba3272951eefeb6eb`  
		Last Modified: Tue, 23 May 2023 09:33:51 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292412d24d01762f2db041e581d2c6d086945b3eee5882453dddd1810ff429a5`  
		Last Modified: Tue, 23 May 2023 09:33:51 GMT  
		Size: 3.7 MB (3717571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8fca81b2bd90d2a54b2623fcde47b23ce03175854fdf6b90e94f6587f62523`  
		Last Modified: Tue, 23 May 2023 09:33:50 GMT  
		Size: 1.4 MB (1438995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e16127d4b4947aed888eb5a36bbd4fbbecde4a613276cc8d335721cd028238`  
		Last Modified: Tue, 23 May 2023 09:33:50 GMT  
		Size: 8.0 MB (8045503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfe5433585b43e3588f0878b9659bf61d17150a194be7b32dac7cb955d6fc62`  
		Last Modified: Tue, 23 May 2023 09:33:49 GMT  
		Size: 1.1 MB (1131300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f781ed4d73c6efc44d512432b1111ea6f5ca556a958da608ee48fbbfd204bb`  
		Last Modified: Tue, 23 May 2023 09:33:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b5b41ab83609241339b72328bc82eac8a4113f56bf2512f07c7daefdd4a27d`  
		Last Modified: Tue, 23 May 2023 09:33:48 GMT  
		Size: 3.2 KB (3194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf02bf579b29da958a9036db57772f40b4aaea9703bbdf8c4d696994bb176ae`  
		Last Modified: Tue, 23 May 2023 09:33:59 GMT  
		Size: 86.0 MB (85962766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2780aa59f36bf2042904f246504e9525670b0d9aeef398e4266f81984452a65`  
		Last Modified: Tue, 23 May 2023 09:33:46 GMT  
		Size: 9.8 KB (9790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c11af0deff60cb86db8122c787d32279715ee13de3ae91894ebff86877c082c`  
		Last Modified: Tue, 23 May 2023 09:33:46 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68445ada246793505ce29e3ce26879e6c34e340b654d1627574f6b21a11daa2`  
		Last Modified: Tue, 23 May 2023 09:33:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d636a605f6c8414e4f6496dac03f949d12d12f7e3877fb58ec0b16d12fef5c06`  
		Last Modified: Tue, 23 May 2023 09:33:46 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:f0bbfe029221661d937d12ecec317a935f79dc37688ecc3c1983fd02c6555336
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134034862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38da3d5fc5bf4bbb51217c7a37394941f3b08da4865c4070b2a63f493cc8810b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:29:26 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 23 May 2023 05:29:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:29:33 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 05:29:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 05:29:46 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 23 May 2023 05:29:47 GMT
ENV LANG=en_US.utf8
# Tue, 23 May 2023 05:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:29:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 05:29:52 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 05:29:52 GMT
ENV PG_MAJOR=15
# Tue, 23 May 2023 05:29:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 23 May 2023 05:29:52 GMT
ENV PG_VERSION=15.3-1.pgdg110+1
# Tue, 23 May 2023 05:30:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 23 May 2023 05:30:11 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 23 May 2023 05:30:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 23 May 2023 05:30:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 23 May 2023 05:30:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 23 May 2023 05:30:12 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 23 May 2023 05:30:12 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 23 May 2023 05:30:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 05:30:12 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 05:30:12 GMT
EXPOSE 5432
# Tue, 23 May 2023 05:30:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f1771724c29194c234b64f364321beedd55d090d083da9750a398a397ca8c1`  
		Last Modified: Tue, 23 May 2023 05:32:23 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fc2ebafa9d04aab151cdcc556184db1e3cc36bd69a0d44b04becf3b8937f7e`  
		Last Modified: Tue, 23 May 2023 05:32:23 GMT  
		Size: 4.4 MB (4416361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc18e8488e52e6a1cfcf7671b3f6e008f075d26acaf0adb6caef54c659b7617b`  
		Last Modified: Tue, 23 May 2023 05:32:22 GMT  
		Size: 1.4 MB (1403318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744912dd5db4a9d402a1e206be183557f117c88701675ed3190de4be6985a2fe`  
		Last Modified: Tue, 23 May 2023 05:32:22 GMT  
		Size: 8.0 MB (8045522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d765f36c95802e7e5f2331d46ac4bfa06dff90fade26435b67644ba92d794abd`  
		Last Modified: Tue, 23 May 2023 05:32:21 GMT  
		Size: 1.2 MB (1249302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0deca2eaaf34cfa3df65c0cc80df4dd56560c12e991f73e8733a9979a45c1c14`  
		Last Modified: Tue, 23 May 2023 05:32:20 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e03cc9013528434e0e26a3f0e1dd4f6eddf34915da61afa1a4538f75dc3cdc`  
		Last Modified: Tue, 23 May 2023 05:32:20 GMT  
		Size: 3.2 KB (3202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20066ef1999e3b9a84dd0bef11a95cc5eac2ee1d9ca25ed848523ac4464dc8ec`  
		Last Modified: Tue, 23 May 2023 05:32:27 GMT  
		Size: 88.8 MB (88847555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c105eabe8a05a0ef616875db76f1ed13750fe38fa5b6d1b54be86422b4ea8657`  
		Last Modified: Tue, 23 May 2023 05:32:18 GMT  
		Size: 9.8 KB (9786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8019485aff47cdf3c1086d18a2c6c842562ebbb56bae9e52eb744b26c4511608`  
		Last Modified: Tue, 23 May 2023 05:32:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbb9b95fe5857529b6b87dce64c2dd1d3c54f49ed86d8bc504297e3c07da277`  
		Last Modified: Tue, 23 May 2023 05:32:18 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bed6a88c898931a3bdcb74f78ef1ee8d1a0971e64fc4cdab799ed2ec5592902`  
		Last Modified: Tue, 23 May 2023 05:32:18 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:4078d653e10cf827d7d0abe46a5cad4aa6d4db1fb8f982f7bb094db3576840c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141051106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:195df7138a43a4835be30293afbb089ea03aa59c2ab5f4289d7f7a5c679f2057`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 03 May 2023 00:00:58 GMT
ADD file:caea439e2dbe0148904e3b9a0c5a843d2d0b7c196725d2b41790594e64dcdce8 in / 
# Wed, 03 May 2023 00:00:58 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:18:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 03 May 2023 00:18:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 00:18:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 03 May 2023 00:18:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 May 2023 00:19:06 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 03 May 2023 00:19:07 GMT
ENV LANG=en_US.utf8
# Wed, 03 May 2023 00:19:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 00:19:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 May 2023 00:19:13 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 03 May 2023 00:19:13 GMT
ENV PG_MAJOR=15
# Wed, 03 May 2023 00:19:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 11 May 2023 23:23:49 GMT
ENV PG_VERSION=15.3-1.pgdg110+1
# Thu, 11 May 2023 23:39:00 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 11 May 2023 23:39:02 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 11 May 2023 23:39:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 11 May 2023 23:39:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 11 May 2023 23:39:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 11 May 2023 23:39:03 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 11 May 2023 23:39:03 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 11 May 2023 23:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 23:39:03 GMT
STOPSIGNAL SIGINT
# Thu, 11 May 2023 23:39:04 GMT
EXPOSE 5432
# Thu, 11 May 2023 23:39:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:10b34014bd1c165cc57a10e7492f17dce658513b7329319fe6c193c85bf752db`  
		Last Modified: Wed, 03 May 2023 00:05:12 GMT  
		Size: 32.4 MB (32388208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b35ed51d471f3560eb7b2df9d2f7aadc58666ea02283ac73153a273fe203812`  
		Last Modified: Wed, 03 May 2023 01:30:22 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6495cb0bb70dfbe8526e349b0b4ab8dddc30fe7c94418128d8d3574254fe3f98`  
		Last Modified: Wed, 03 May 2023 01:30:23 GMT  
		Size: 4.8 MB (4813623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186341ba2ed25efdfbd36b4a4c9b824e92063c2d8a6b4b101bcb58a4fc79f568`  
		Last Modified: Wed, 03 May 2023 01:30:22 GMT  
		Size: 1.4 MB (1447121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c1fdf3f4df0df87f994e24cc75b175d0d2fb07efa962caa3f053814d277957`  
		Last Modified: Wed, 03 May 2023 01:30:22 GMT  
		Size: 8.0 MB (8045317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e330a427315ad194c6097682cb5015b8721b19be250df94ffefde1f4ae468c9`  
		Last Modified: Wed, 03 May 2023 01:30:20 GMT  
		Size: 1.3 MB (1251741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3d3de83f88c711a1c86389b04d4d0fae11f7528087a377c50716abdb0f6cf5`  
		Last Modified: Wed, 03 May 2023 01:30:19 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad32a444a313868d8017fe49b81383f522baea2d2d2da52bd5f2505117dc5f5`  
		Last Modified: Wed, 03 May 2023 01:30:19 GMT  
		Size: 3.2 KB (3197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3a9b3b7a4753d8b0ee41ddbc64c152324b74643eeba998f8cef726a280222b`  
		Last Modified: Fri, 12 May 2023 00:59:54 GMT  
		Size: 93.1 MB (93085056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac5ea6b682de10882bb515418c0a83a220b9ab62ccb93089e9ecb8b8e7ce8f`  
		Last Modified: Fri, 12 May 2023 00:59:37 GMT  
		Size: 9.8 KB (9781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453da5001713488cb5dcd5677131f00814a00485531eb6231317746612e30a80`  
		Last Modified: Fri, 12 May 2023 00:59:36 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e967195e0b99d1fb89a9bd5358a1f660fffa7334e3209ff16542c080dc8522`  
		Last Modified: Fri, 12 May 2023 00:59:36 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a456034078954414dc17cc2a5fcde91ff0ce02aed35d73b7257b1453333351d`  
		Last Modified: Fri, 12 May 2023 00:59:36 GMT  
		Size: 4.8 KB (4792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:7b65d3b8c575ec4920959d96801a313955cd9e78bfbca3e1001a008458dbb162
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133329391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61986ee385421c599fe638383e91784a8ed74f24361ad8f553ac424b22b7bbb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 02 May 2023 23:49:45 GMT
ADD file:c3427ec4e3a2c988fdd372b529660d45ee105e317d6a964ce96f8f9009a3c21e in / 
# Tue, 02 May 2023 23:49:49 GMT
CMD ["bash"]
# Wed, 03 May 2023 05:15:37 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 03 May 2023 05:16:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 05:16:17 GMT
ENV GOSU_VERSION=1.16
# Wed, 03 May 2023 05:16:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 May 2023 05:17:21 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 03 May 2023 05:17:24 GMT
ENV LANG=en_US.utf8
# Wed, 03 May 2023 05:17:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 05:17:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 03 May 2023 05:17:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 03 May 2023 05:17:55 GMT
ENV PG_MAJOR=15
# Wed, 03 May 2023 05:17:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 11 May 2023 21:27:06 GMT
ENV PG_VERSION=15.3-1.pgdg110+1
# Thu, 11 May 2023 22:27:46 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 11 May 2023 22:27:52 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 11 May 2023 22:27:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 11 May 2023 22:28:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 11 May 2023 22:28:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 11 May 2023 22:28:10 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 11 May 2023 22:28:13 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 11 May 2023 22:28:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 22:28:19 GMT
STOPSIGNAL SIGINT
# Thu, 11 May 2023 22:28:22 GMT
EXPOSE 5432
# Thu, 11 May 2023 22:28:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:498edd615f8781385e0d5246e189d80b5caceb207fe26608a12605d0a823d4df`  
		Last Modified: Tue, 02 May 2023 23:58:10 GMT  
		Size: 29.6 MB (29623482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce7218f38e4902b36a55ec97adc47fb24c4836c776b2106fd27aa398aebdf4d`  
		Last Modified: Wed, 03 May 2023 10:12:08 GMT  
		Size: 1.7 KB (1661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0a5f6f6c8717c2d3ee5a26cb6d093fb02d85a9147b10b9a2f1eec26af460fb`  
		Last Modified: Wed, 03 May 2023 10:12:12 GMT  
		Size: 4.2 MB (4196364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db0842d2a2b3ac6971b300f373a61a6951ebee21b93eb089447fa8b83ef6227`  
		Last Modified: Wed, 03 May 2023 10:12:09 GMT  
		Size: 1.4 MB (1358441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f540a5846b9a641da3bd11e4e10a3a97c2741c0b3e7a78efe1225efb19ce9a1b`  
		Last Modified: Wed, 03 May 2023 10:12:13 GMT  
		Size: 8.0 MB (8044027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7595f8837bd017b71b37a280038ebd228bc193ce67b93d7dd457cb709f37e760`  
		Last Modified: Wed, 03 May 2023 10:12:06 GMT  
		Size: 1.1 MB (1089590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599cbf9e01724160a672088c36cbdcb4cc3b4e795321a9c62159182915dec769`  
		Last Modified: Wed, 03 May 2023 10:12:05 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aac1197805b2936708786cb30f2d6d222e827b474ed616f03c3dbbaa63c76ed`  
		Last Modified: Wed, 03 May 2023 10:12:05 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236a696069ce2ed9f5a9bb95a0eeb472e328a2f86e1a2af81a645c70cd2894a6`  
		Last Modified: Fri, 12 May 2023 02:16:55 GMT  
		Size: 89.0 MB (88997689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e5d0be262497d3c9744265687e0d2b15fc20149752861a644c42fc1059503d`  
		Last Modified: Fri, 12 May 2023 02:16:00 GMT  
		Size: 9.8 KB (9789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed04bb8ec5f392a0edc67b3583521cc89997d88d5e964b68bc5fe5de4a3bfd77`  
		Last Modified: Fri, 12 May 2023 02:15:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2ce5e834ee3bef40030416d238a3c2b5e4bf9f494b70d1d43ac226dabe7eb3`  
		Last Modified: Fri, 12 May 2023 02:15:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01657757df7a4acda38b9e75928672eb3671e4f1fd25106d3fbc6f1f99d40be`  
		Last Modified: Fri, 12 May 2023 02:15:59 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:850aba54c940d45541cadee7de39d3ce5e19d46056cd8f1b49518144ed2244d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.0 MB (148039202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fe687d3a129326efd760b116a01e948b4ee25a55359d348942ba118083bde8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 23 May 2023 01:17:35 GMT
ADD file:719aea085739ec41c255f35070ca652d4e356c5ee62c8237f8ebc7389feb8e38 in / 
# Tue, 23 May 2023 01:17:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:34:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 23 May 2023 04:35:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:35:05 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 04:35:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 04:35:31 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 23 May 2023 04:35:31 GMT
ENV LANG=en_US.utf8
# Tue, 23 May 2023 04:35:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:35:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 04:35:42 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 04:35:43 GMT
ENV PG_MAJOR=15
# Tue, 23 May 2023 04:35:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 23 May 2023 04:35:43 GMT
ENV PG_VERSION=15.3-1.pgdg110+1
# Tue, 23 May 2023 04:36:28 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 23 May 2023 04:36:32 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 23 May 2023 04:36:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 23 May 2023 04:36:34 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 23 May 2023 04:36:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 23 May 2023 04:36:35 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 23 May 2023 04:36:35 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 23 May 2023 04:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:36:36 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 04:36:36 GMT
EXPOSE 5432
# Tue, 23 May 2023 04:36:36 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b6c83d2f160e7e38990586d26caa105ff577368a887fd754ae4634cdbfec83ff`  
		Last Modified: Tue, 23 May 2023 01:22:03 GMT  
		Size: 35.3 MB (35280911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e32c10e0d25cfde474630b1111361aa90bc2f7e52064495d66c5ecb438cfec`  
		Last Modified: Tue, 23 May 2023 04:41:32 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b54236bfc967cacf19ce25419cd2876f4d70ff825acb2ed1e9dbe2af71ba437`  
		Last Modified: Tue, 23 May 2023 04:41:33 GMT  
		Size: 5.2 MB (5222890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb0a2677c278c33654e025bc97731dc9caec439ef213674d93ce6dff160193e`  
		Last Modified: Tue, 23 May 2023 04:41:32 GMT  
		Size: 1.4 MB (1393318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9414fd0feffa941cebf57445978ced0cbd1dee02558a3ea404bbd72762f067c5`  
		Last Modified: Tue, 23 May 2023 04:41:32 GMT  
		Size: 8.0 MB (8045575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d2e69bc8e692408f766ecb404132f911880791dcf62aa8165b5489246c9b34`  
		Last Modified: Tue, 23 May 2023 04:41:30 GMT  
		Size: 1.4 MB (1420204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3348c0d852664b52e64cddf114b84826202ceb86a946e4181aee7a306abafe`  
		Last Modified: Tue, 23 May 2023 04:41:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428fe0c6f32852085628aa1d26d2c8701c34c20eb17d746c039a8d6f13628ae9`  
		Last Modified: Tue, 23 May 2023 04:41:29 GMT  
		Size: 3.2 KB (3203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448ac81dd3d89c02770e9311c16124f8454f007c2cdb25e18d5c767fc9232ba2`  
		Last Modified: Tue, 23 May 2023 04:41:50 GMT  
		Size: 96.7 MB (96656250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc5c399feca3bbf9a4369cace96296d999a1da906d963232b6cf6a5577ae144`  
		Last Modified: Tue, 23 May 2023 04:41:27 GMT  
		Size: 9.8 KB (9782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7f5ff5daffd9dde14465e512b5022c507f35263d388becdb0e7ac46eb1aab5`  
		Last Modified: Tue, 23 May 2023 04:41:27 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b848f896c1eea1ccf133811baf3d6bf5d506030d4bd4fb1833b9f7e902761f`  
		Last Modified: Tue, 23 May 2023 04:41:27 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad14c78cbd713fa73957732080afa98772db04b49fda85442be14987a4e1f5b`  
		Last Modified: Tue, 23 May 2023 04:41:27 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:be8073adcf522c44e042c16d68d406564a56b36f012d91cd034e14ac96938310
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142578389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa1224acfc37dd0b33f287809620b45a0d789a16289ec92b2c67396d6499a8f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 03:43:45 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 23 May 2023 03:43:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:43:49 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 03:43:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 03:44:01 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 23 May 2023 03:44:01 GMT
ENV LANG=en_US.utf8
# Tue, 23 May 2023 03:44:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 03:44:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 03:44:06 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 03:44:06 GMT
ENV PG_MAJOR=15
# Tue, 23 May 2023 03:44:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 23 May 2023 03:44:06 GMT
ENV PG_VERSION=15.3-1.pgdg110+1
# Tue, 23 May 2023 03:44:26 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 23 May 2023 03:44:30 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 23 May 2023 03:44:31 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 23 May 2023 03:44:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 23 May 2023 03:44:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 23 May 2023 03:44:31 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 23 May 2023 03:44:31 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 23 May 2023 03:44:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 03:44:32 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 03:44:32 GMT
EXPOSE 5432
# Tue, 23 May 2023 03:44:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634dbfcfbccb434a9ff3c6f1cbe19eedb2e98de82ca84471ce281f3e62bfc32f`  
		Last Modified: Tue, 23 May 2023 03:47:44 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d7b8031b5469735cb7bb06401bfda894a639cc90aef8fc1cb9c223bff424b4`  
		Last Modified: Tue, 23 May 2023 03:47:44 GMT  
		Size: 4.3 MB (4302383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78560232cf094a7503a58e697efdcf5fcb7310d2b1bfdae63674f9c043965b67`  
		Last Modified: Tue, 23 May 2023 03:47:44 GMT  
		Size: 1.4 MB (1437222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f1b63baae033792e892c9f9395997406ab7877e5784e9e9d1774d2e3337d28`  
		Last Modified: Tue, 23 May 2023 03:47:44 GMT  
		Size: 8.1 MB (8099208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7875504344a7d712417418db4c5f1e5383bea79e1e26066b05f2c8a61e01450`  
		Last Modified: Tue, 23 May 2023 03:47:43 GMT  
		Size: 1.2 MB (1238057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013b5a1d1a685e498efdaf016b4b81095a4dcc7d981088633902120f61efaba8`  
		Last Modified: Tue, 23 May 2023 03:47:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c76b8dda32cda9e44bc66006a9c064f330bded5ecdc97813a5fc0b5f77051a`  
		Last Modified: Tue, 23 May 2023 03:47:42 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd17d53b123513e5d43dbdb5123a6f5e59139f6307e38a1e22d6071177d18db`  
		Last Modified: Tue, 23 May 2023 03:47:53 GMT  
		Size: 97.8 MB (97839295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d201be294fd3705d705d148ebdd48bb08edb3f3999a2678e97bef5e2030c40`  
		Last Modified: Tue, 23 May 2023 03:47:41 GMT  
		Size: 9.8 KB (9785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb0e4078917ea4783d5501795066f6be4e8960d6b46d1bd263c6759131f8a0a`  
		Last Modified: Tue, 23 May 2023 03:47:41 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cfe74cfc61a8b17674a92408ebfe64cf5509e590577c8549d9b66966c1d60e`  
		Last Modified: Tue, 23 May 2023 03:47:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974af97129296d3fa0b97520c4e8c2741f0bc7d3110681edb7183e6db4421ef8`  
		Last Modified: Tue, 23 May 2023 03:47:41 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
