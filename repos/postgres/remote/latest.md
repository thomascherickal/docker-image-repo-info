## `postgres:latest`

```console
$ docker pull postgres@sha256:ab0be6280ada8549f45e6662ab4f00b7f601886fcd55c5976565d4636d87c8b2
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

### `postgres:latest` - linux; amd64

```console
$ docker pull postgres@sha256:625df66e2b092d2a5be485d52f80d6edf41cb02f7315a29c980a877519d14e4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137800229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b0c105737a84fd66dc0fbe8e6cf670eba092c9bcdd02430ad059615372376f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:55:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 12:55:03 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 20 Apr 2022 12:55:03 GMT
ENV GOSU_VERSION=1.14
# Wed, 20 Apr 2022 12:55:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 20 Apr 2022 12:55:18 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 20 Apr 2022 12:55:18 GMT
ENV LANG=en_US.utf8
# Wed, 20 Apr 2022 12:55:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:55:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 20 Apr 2022 12:55:24 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 20 Apr 2022 12:55:24 GMT
ENV PG_MAJOR=14
# Wed, 20 Apr 2022 12:55:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Wed, 20 Apr 2022 12:55:24 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Wed, 20 Apr 2022 12:55:42 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 20 Apr 2022 12:55:43 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 20 Apr 2022 12:55:44 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 20 Apr 2022 12:55:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 20 Apr 2022 12:55:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 20 Apr 2022 12:55:44 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 20 Apr 2022 12:55:44 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 20 Apr 2022 12:55:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 12:55:45 GMT
STOPSIGNAL SIGINT
# Wed, 20 Apr 2022 12:55:45 GMT
EXPOSE 5432
# Wed, 20 Apr 2022 12:55:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bb685f623fe10169c69d4ec74547c0dd090744f323a73e91ec298ae49198cd`  
		Last Modified: Wed, 20 Apr 2022 12:59:51 GMT  
		Size: 4.4 MB (4414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3027ff70541005e6dc087e541c306590f84da7ab2737fa8ee9e4acb2ef7b54d8`  
		Last Modified: Wed, 20 Apr 2022 12:59:49 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062371e3461d10dd17b37b174c5204709e4a828de004ae80ef44a9776c3b693a`  
		Last Modified: Wed, 20 Apr 2022 12:59:50 GMT  
		Size: 1.4 MB (1418390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d54e944de74ab373566c980af765f066053a6c2f12274a7ee808e7cfc56158`  
		Last Modified: Wed, 20 Apr 2022 12:59:49 GMT  
		Size: 8.0 MB (8045308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6530357dda9a856600bb73f3894189a51697b46e7ddaac67782bc3fa150f3d6c`  
		Last Modified: Wed, 20 Apr 2022 12:59:48 GMT  
		Size: 1.3 MB (1261153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d302dc78c63f82eeaf3acc796a480b1c2ba421d011a73e7ea03a2f629bf86d`  
		Last Modified: Wed, 20 Apr 2022 12:59:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d91cb1d3c135c4731590eb6940aa236226e03bc47569827209a515fcc7a085`  
		Last Modified: Wed, 20 Apr 2022 12:59:47 GMT  
		Size: 3.2 KB (3196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbd62b0af2872ac19989dd6d99985e04efad1768505c10bced7b7dcf5b1b65f`  
		Last Modified: Wed, 20 Apr 2022 12:59:57 GMT  
		Size: 91.3 MB (91262190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfdfc8fbef3077a84eab008599ccf444967f5dc6c8b8bac3c40421ac6b2f5c2`  
		Last Modified: Wed, 20 Apr 2022 12:59:45 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635f8fae1d0617c496c561c228d8642c2c4823d945c647cf6a6ffb8e6c7cc7a0`  
		Last Modified: Wed, 20 Apr 2022 12:59:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b6711661dda05f9b7808313c5467d8cfd56c8f2d9903307a181457544b2b2d`  
		Last Modified: Wed, 20 Apr 2022 12:59:44 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08147da7b54ad4311cf3ebb22f8d68da5e5c67b911ba6cef66126605a55f501`  
		Last Modified: Wed, 20 Apr 2022 12:59:44 GMT  
		Size: 4.7 KB (4693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v5

```console
$ docker pull postgres@sha256:cc10c993c51e762b7f3ab8d6afcda7f725c5c8bad4fb9a40c5c887dcffa4d6bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131130792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9391a9cd9721f788be76ea27aed83f741aca6fd536142c06ec39b71336becacf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 07:16:42 GMT
ADD file:f20c57847025604e1ea1a848af3f090f71d78b5fc2eb2ac795822da94d6e6a0a in / 
# Wed, 20 Apr 2022 07:16:43 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 02:37:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Apr 2022 02:37:19 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 21 Apr 2022 02:37:20 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Apr 2022 02:37:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Apr 2022 02:38:06 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 21 Apr 2022 02:38:07 GMT
ENV LANG=en_US.utf8
# Thu, 21 Apr 2022 02:38:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 02:38:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Apr 2022 02:38:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 21 Apr 2022 02:38:23 GMT
ENV PG_MAJOR=14
# Thu, 21 Apr 2022 02:38:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 21 Apr 2022 02:38:24 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Thu, 21 Apr 2022 03:16:44 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 21 Apr 2022 03:16:46 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 21 Apr 2022 03:16:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 21 Apr 2022 03:16:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 21 Apr 2022 03:16:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 21 Apr 2022 03:16:50 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 21 Apr 2022 03:16:51 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Thu, 21 Apr 2022 03:16:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 03:16:51 GMT
STOPSIGNAL SIGINT
# Thu, 21 Apr 2022 03:16:52 GMT
EXPOSE 5432
# Thu, 21 Apr 2022 03:16:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3edd9d296fa023e00f76828c9d6fd6cc5b03e626341a6a045c40d2ea16c32d08`  
		Last Modified: Wed, 20 Apr 2022 07:32:27 GMT  
		Size: 28.9 MB (28921085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e2b49f054c7fb25bec9edd1fde10be69232ec8ec67d62fae72cab1df280adc`  
		Last Modified: Thu, 21 Apr 2022 06:25:32 GMT  
		Size: 4.1 MB (4096548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f281c7788d94b9cc380ffc0ea286caaa86d44d9f40de23fb73640b418b9f23`  
		Last Modified: Thu, 21 Apr 2022 06:25:28 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5986160cfc18a16b14c0b667589d171c1eff85cf9425414d1c0f098dd59e0522`  
		Last Modified: Thu, 21 Apr 2022 06:25:29 GMT  
		Size: 1.4 MB (1382627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd6bcc78e483c6cd7297f6a43c77bc2a1cff5cd87cbd2cc8415a065b8b34717`  
		Last Modified: Thu, 21 Apr 2022 06:25:33 GMT  
		Size: 8.0 MB (8045293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48500581cdfa21f31ae7ec93415ffcae29538e2414657d0a0a7e1266bf1b1394`  
		Last Modified: Thu, 21 Apr 2022 06:25:27 GMT  
		Size: 1.3 MB (1257318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b1ef8fb61ed9648230778e298a54ec0997bd48aaed717c1296120deb9f0f0b`  
		Last Modified: Thu, 21 Apr 2022 06:25:26 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87cc92186fe72e6cdf63f8907008a4b2d8739fb2d25bd874de7df9ec7135d00`  
		Last Modified: Thu, 21 Apr 2022 06:25:26 GMT  
		Size: 3.2 KB (3202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3306c110f93c1e6911e7c372b2b2bb352937f0467842dc445190d61d23307af`  
		Last Modified: Thu, 21 Apr 2022 06:26:20 GMT  
		Size: 87.4 MB (87408216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5368ef306cbfcc38d9948719fbf387bd20aec12ec045cdf600ee7daff81b6690`  
		Last Modified: Thu, 21 Apr 2022 06:25:24 GMT  
		Size: 9.5 KB (9538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c36cff8849353cb945d25ae4979fe7c6dda25877ea89ce2bfe673f0fe774444`  
		Last Modified: Thu, 21 Apr 2022 06:25:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499c4fa0e3a6b44a8a5995bedc884a9391ee432f63845c371130d300ccb58069`  
		Last Modified: Thu, 21 Apr 2022 06:25:25 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508f5eaf12f38162d7cdb6f4794779c95a9f6ee92e06aacea3740e490662b633`  
		Last Modified: Thu, 21 Apr 2022 06:25:24 GMT  
		Size: 4.7 KB (4696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v7

```console
$ docker pull postgres@sha256:472a16bddda81b2f9814b056645f63045d5e4990e27fc99e485a81751cbdd88d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125779215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee1b6051fbe74d18830f86cc467e1c89a08dc6ca0837f15dcd0c54713e16a893`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 06:23:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Apr 2022 06:23:25 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 21 Apr 2022 06:23:26 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Apr 2022 06:23:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Apr 2022 06:24:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 21 Apr 2022 06:24:05 GMT
ENV LANG=en_US.utf8
# Thu, 21 Apr 2022 06:24:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 06:24:16 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Apr 2022 06:24:18 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 21 Apr 2022 06:24:18 GMT
ENV PG_MAJOR=14
# Thu, 21 Apr 2022 06:24:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 21 Apr 2022 06:24:19 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Thu, 21 Apr 2022 06:58:32 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 21 Apr 2022 06:58:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 21 Apr 2022 06:58:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 21 Apr 2022 06:58:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 21 Apr 2022 06:58:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 21 Apr 2022 06:58:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 21 Apr 2022 06:58:38 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Thu, 21 Apr 2022 06:58:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 06:58:39 GMT
STOPSIGNAL SIGINT
# Thu, 21 Apr 2022 06:58:40 GMT
EXPOSE 5432
# Thu, 21 Apr 2022 06:58:40 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae91ea7162f2ed8974b56c55e84be1415aafeb65a2b4ee532bd53e8b858da2d6`  
		Last Modified: Thu, 21 Apr 2022 09:50:20 GMT  
		Size: 3.7 MB (3717255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a225ae1d08772ff552e11e8259a01a32cb0c760ecc2ab0cebecd6e6f9dcdeb1a`  
		Last Modified: Thu, 21 Apr 2022 09:50:17 GMT  
		Size: 1.8 KB (1793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5135069f8a2e46f72ea34e6aeaf28f79f7060c134fd0b78dec3cd6627906cf22`  
		Last Modified: Thu, 21 Apr 2022 09:50:18 GMT  
		Size: 1.4 MB (1375335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e36cb2927d7a31b0e9dc2f629a276148ae7f65cb68526df0b7ed9e63007aea`  
		Last Modified: Thu, 21 Apr 2022 09:50:22 GMT  
		Size: 8.0 MB (8045405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6edb7db1e252a4e8073ac37c46f3599715585f705cc3b50fa9c1b23ba0f833c`  
		Last Modified: Thu, 21 Apr 2022 09:50:16 GMT  
		Size: 1.1 MB (1131210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08ab87ae4f0ac90c80b35832b217d05830653b19ce16ea257e87750fbd0476c`  
		Last Modified: Thu, 21 Apr 2022 09:50:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b77220fab8955b44d1944de26d475595ce0edd27cbed5904125a1967288b04`  
		Last Modified: Thu, 21 Apr 2022 09:50:15 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae5538138bf76415f96f22c578cc76aa619ee5137f1a94b266027007fe92b9c`  
		Last Modified: Thu, 21 Apr 2022 09:51:05 GMT  
		Size: 84.9 MB (84914540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710262e6196ea653ecfaa29bcf7ff1021482e8b1d4bab2916a5e9a1f7fb3dad9`  
		Last Modified: Thu, 21 Apr 2022 09:50:13 GMT  
		Size: 9.5 KB (9540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395d4ed02571954c11c2c546077b919abe54492bd4cae0e158c62b4b6f0082be`  
		Last Modified: Thu, 21 Apr 2022 09:50:14 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d756a410b5bab904e2ecb920d04ffd831f6d0b7ac1beb6dcf21a6cb0e932b740`  
		Last Modified: Thu, 21 Apr 2022 09:50:14 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f370d2193a8d6485fcc60b5f950928263ac110b2d8c6845352ada30a9b795d`  
		Last Modified: Thu, 21 Apr 2022 09:50:14 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:59952e5e27a9852766a88e52885c88367300d0f15202844aaad5a9361b868856
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132509447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95700231f9c263702da9a25447346a9477b0298ea5f174c3f880bb63be5eac08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:04:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 11:04:08 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 20 Apr 2022 11:04:09 GMT
ENV GOSU_VERSION=1.14
# Wed, 20 Apr 2022 11:04:18 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 20 Apr 2022 11:04:24 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 20 Apr 2022 11:04:25 GMT
ENV LANG=en_US.utf8
# Wed, 20 Apr 2022 11:04:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:04:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 20 Apr 2022 11:04:33 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 20 Apr 2022 11:04:33 GMT
ENV PG_MAJOR=14
# Wed, 20 Apr 2022 11:04:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Wed, 20 Apr 2022 11:04:35 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Wed, 20 Apr 2022 11:04:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 20 Apr 2022 11:04:56 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 20 Apr 2022 11:04:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 20 Apr 2022 11:04:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 20 Apr 2022 11:04:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 20 Apr 2022 11:05:00 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 20 Apr 2022 11:05:02 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 20 Apr 2022 11:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 11:05:03 GMT
STOPSIGNAL SIGINT
# Wed, 20 Apr 2022 11:05:04 GMT
EXPOSE 5432
# Wed, 20 Apr 2022 11:05:05 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843e625c486cadb68ed5db239f94a5bfefe69335abdff9122be56042f4a64661`  
		Last Modified: Wed, 20 Apr 2022 11:28:52 GMT  
		Size: 4.2 MB (4208995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66c9c6dcbdb495ad23e9de8cd7f98acb251ffa463e8d2177192a27d072e9193`  
		Last Modified: Wed, 20 Apr 2022 11:28:51 GMT  
		Size: 1.6 KB (1649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf8d7ef83529fedcd9178f98e342888ff9ff7b0af9971f18e86eaed41f25aac`  
		Last Modified: Wed, 20 Apr 2022 11:28:51 GMT  
		Size: 1.3 MB (1346123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad047717fcf187a7f7db96e09169dea6cb6245159516c3ea46179077950ab24`  
		Last Modified: Wed, 20 Apr 2022 11:28:50 GMT  
		Size: 8.0 MB (8043519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dc9f6b717aeb020f1ca6e1f4f4bf534af1cec19647bfb8464da61fd1f48608`  
		Last Modified: Wed, 20 Apr 2022 11:28:49 GMT  
		Size: 1.0 MB (1025851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040ef4050a502d7e96c07286c55cb18cd0b5fcccb2f0e93dc84d7a02a9184f99`  
		Last Modified: Wed, 20 Apr 2022 11:28:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf36b8f8c41fd56e191e03e9b69c689a422341ce6e40028012c65b0506fe2a`  
		Last Modified: Wed, 20 Apr 2022 11:28:49 GMT  
		Size: 3.1 KB (3138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281af44b7af00cc988fed7bec08000d60d1d6cb04c5dc168126a38c2587a91e4`  
		Last Modified: Wed, 20 Apr 2022 11:28:59 GMT  
		Size: 87.8 MB (87799737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67794bd34d7c75cd68621d6afce0a7e96f7dc2f8172f408fce4af489c98997a`  
		Last Modified: Wed, 20 Apr 2022 11:28:46 GMT  
		Size: 9.5 KB (9525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84bed0948707b2c73a4e13705dcf4bc2685135aedf53ddb8126c6640de44bc0`  
		Last Modified: Wed, 20 Apr 2022 11:28:46 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea9db95f9079f3cf5f304ce60fca7fccc9433bdd6ade42e50d23e5476822d7b`  
		Last Modified: Wed, 20 Apr 2022 11:28:46 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feae5691bf7739d424ee31211836a76168ca85ba57340abcecbfea52b86a8fe5`  
		Last Modified: Wed, 20 Apr 2022 11:28:47 GMT  
		Size: 4.7 KB (4693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; 386

```console
$ docker pull postgres@sha256:cf25a7ce07354cdfdc9f78124f2606b6d903dc0b3a70beb5c6cd14811b702f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139482021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e074ad59946471584a8b348f0080a5826f092d4d3b5bd2e34d5d54ca76525b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 07:37:35 GMT
ADD file:460761e2baaea91893a907ce122ff7d585ef5704f48c03454835986028a1d842 in / 
# Wed, 20 Apr 2022 07:37:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 14:45:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 14:45:15 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 20 Apr 2022 14:45:16 GMT
ENV GOSU_VERSION=1.14
# Wed, 20 Apr 2022 14:45:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 20 Apr 2022 14:45:32 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 20 Apr 2022 14:45:32 GMT
ENV LANG=en_US.utf8
# Wed, 20 Apr 2022 14:45:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 14:45:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 20 Apr 2022 14:45:40 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 20 Apr 2022 14:45:41 GMT
ENV PG_MAJOR=14
# Wed, 20 Apr 2022 14:45:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Wed, 20 Apr 2022 14:45:43 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Wed, 20 Apr 2022 14:59:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 20 Apr 2022 14:59:04 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 20 Apr 2022 14:59:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 20 Apr 2022 14:59:06 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 20 Apr 2022 14:59:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 20 Apr 2022 14:59:08 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 20 Apr 2022 14:59:10 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 20 Apr 2022 14:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 14:59:11 GMT
STOPSIGNAL SIGINT
# Wed, 20 Apr 2022 14:59:12 GMT
EXPOSE 5432
# Wed, 20 Apr 2022 14:59:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6e5c4eb151e267d273883db6e9aee3ff01be07e098ca33f0d1d65bb0e0416921`  
		Last Modified: Wed, 20 Apr 2022 07:44:54 GMT  
		Size: 32.4 MB (32389597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16066b0a3c095bb9fbec9bd79099d9dbbde0c8095c9a36e14bb3799b378ce4e`  
		Last Modified: Wed, 20 Apr 2022 15:49:35 GMT  
		Size: 4.6 MB (4606844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985c566528a7908b996d416ade2b89fddd0a8d52cfc73cfcb22d6436030f340f`  
		Last Modified: Wed, 20 Apr 2022 15:49:33 GMT  
		Size: 1.6 KB (1642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b470a9fe35d8c0120d8a5c4c8cdc44644b6a096ba70c2d2707d842831e2b9`  
		Last Modified: Wed, 20 Apr 2022 15:49:34 GMT  
		Size: 1.4 MB (1385109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df801a4b47f85e67a95df1d4cc6b1e37acc2ebec28448176ffe39c7239cbf1cc`  
		Last Modified: Wed, 20 Apr 2022 15:49:32 GMT  
		Size: 8.0 MB (8043547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e219420f9293efc074049b589efdc56f46900d72a0be52b4726d4f32bbdc91d`  
		Last Modified: Wed, 20 Apr 2022 15:49:32 GMT  
		Size: 1.0 MB (1027922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97f31ebf8be9ebf4c645f255c56ca585d23b3cb96bbff8499fb9114d60e01e4`  
		Last Modified: Wed, 20 Apr 2022 15:49:31 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a367661aa78b29d5fc68ff7c588c577657c6981228dff870f6e08407982382`  
		Last Modified: Wed, 20 Apr 2022 15:49:31 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10920db89b3a5037386b165804b7880fbaaed72026377f8ab70be4ea01c44662`  
		Last Modified: Wed, 20 Apr 2022 15:49:41 GMT  
		Size: 92.0 MB (92009565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac7dfbdb7af4d780398fade7e0ed97e25714554e7f26d261fa04520ef8a1d33`  
		Last Modified: Wed, 20 Apr 2022 15:49:29 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf7e48890e77d4f5247de2c7e1e163a840042db852a547e91bd529d81b7a2ed`  
		Last Modified: Wed, 20 Apr 2022 15:49:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c898b3e71278ed2295ae4d3b109c26f8df048e828e9c921338d7dd486edc144`  
		Last Modified: Wed, 20 Apr 2022 15:49:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a4de274e2803dd1389f5dbe8f59735c885866cad397ecbf26fe48180047d97`  
		Last Modified: Wed, 20 Apr 2022 15:49:29 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; mips64le

```console
$ docker pull postgres@sha256:405db2d2654b25d1699bbbc43d5d41383d91367eed658c208900e68a317a5405
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132253685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647f783312cb8b64c063a6da423fc2e5f814fbbba150aa66222b947dbd824b4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 14:28:35 GMT
ADD file:11939fa9b6e0a3bde2ba32552130208df232ae0dd139b9244b80fa309690d57f in / 
# Wed, 20 Apr 2022 14:28:39 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 09:28:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Apr 2022 09:28:37 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 21 Apr 2022 09:28:39 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Apr 2022 09:29:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Apr 2022 09:29:41 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 21 Apr 2022 09:29:43 GMT
ENV LANG=en_US.utf8
# Thu, 21 Apr 2022 09:30:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 09:30:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Apr 2022 09:30:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 21 Apr 2022 09:30:16 GMT
ENV PG_MAJOR=14
# Thu, 21 Apr 2022 09:30:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 21 Apr 2022 09:30:21 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Thu, 21 Apr 2022 10:30:20 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 21 Apr 2022 10:30:28 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 21 Apr 2022 10:30:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 21 Apr 2022 10:30:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 21 Apr 2022 10:30:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 21 Apr 2022 10:30:47 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 21 Apr 2022 10:30:50 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Thu, 21 Apr 2022 10:30:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 10:30:57 GMT
STOPSIGNAL SIGINT
# Thu, 21 Apr 2022 10:31:00 GMT
EXPOSE 5432
# Thu, 21 Apr 2022 10:31:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:211e565c951d5d12adf5ac13e34b5fdba747f88e6b462c2863538110b219144c`  
		Last Modified: Wed, 20 Apr 2022 14:39:17 GMT  
		Size: 29.6 MB (29641236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74cd5f51ab8207bde2738103d31974c754548abb4c64861937b1410e5ff8237`  
		Last Modified: Thu, 21 Apr 2022 13:57:55 GMT  
		Size: 4.2 MB (4196172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c5a91db8ebd653cc690d8e943d9db812d76ed555737f960ce982fb22e3d059`  
		Last Modified: Thu, 21 Apr 2022 13:57:51 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745b3f37335a3f751612f985b7faa7b4b46f2f3332e98def2ca55040ee1555ec`  
		Last Modified: Thu, 21 Apr 2022 13:57:52 GMT  
		Size: 1.3 MB (1297991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc3b95704370b7092be0fabdec11b74a4bad0ecfd236c13315008c9a9a71ecc`  
		Last Modified: Thu, 21 Apr 2022 13:57:56 GMT  
		Size: 8.0 MB (8043937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767120112c01a94dde1898f364547eca2cb103f4bb59b873567ee54b53d9d36c`  
		Last Modified: Thu, 21 Apr 2022 13:57:49 GMT  
		Size: 1.1 MB (1089435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61eebd1c1948738c4cd9705861951e95bb2bdc2143dd0cf5c4392a6a99411d0`  
		Last Modified: Thu, 21 Apr 2022 13:57:48 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92feb1191696fd1aa51fb839093ecaa3e1a07ba64f596d22dd9c164941fc80`  
		Last Modified: Thu, 21 Apr 2022 13:57:48 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df33f0babeb136d6289076270e57b9fb0ff5df37d094274f1e6981fa99c6987d`  
		Last Modified: Thu, 21 Apr 2022 13:58:43 GMT  
		Size: 88.0 MB (87965469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42236964d2cb439f0b73b1e131850a9e9cba226c90bf10fd02d57ea524b305fb`  
		Last Modified: Thu, 21 Apr 2022 13:57:46 GMT  
		Size: 9.5 KB (9534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76cef5ee4eaa5892df9106f54d175bc98308b5c529bdf1f3a99adf18166201e`  
		Last Modified: Thu, 21 Apr 2022 13:57:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa0c305cc86ede1802c9495fe9d92c3ba83241f01f1dc6abb0970cf5210fe59`  
		Last Modified: Thu, 21 Apr 2022 13:57:46 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cbd8e67a7e2305cf29df65c2c41b7fd4425413d42987d05c08a85fe3fb174e`  
		Last Modified: Thu, 21 Apr 2022 13:57:46 GMT  
		Size: 4.7 KB (4697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; ppc64le

```console
$ docker pull postgres@sha256:ddb5d0a6805ffc2d1fb9f108952a7564a0aa441673117de584a7557a66674808
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146893276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bea59a62e347fa5289975d12740f09d31b0970401b6e308ab60d460bb307a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 09:46:36 GMT
ADD file:8d406ebce4d9b0884d46ee25ec31fe7714726024b80aba9b408d81d39e2f6f8c in / 
# Wed, 20 Apr 2022 09:46:44 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 03:44:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Apr 2022 03:44:20 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 21 Apr 2022 03:44:22 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Apr 2022 03:44:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 21 Apr 2022 03:45:21 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 21 Apr 2022 03:45:24 GMT
ENV LANG=en_US.utf8
# Thu, 21 Apr 2022 03:45:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 03:45:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Apr 2022 03:45:59 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 21 Apr 2022 03:46:01 GMT
ENV PG_MAJOR=14
# Thu, 21 Apr 2022 03:46:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 21 Apr 2022 03:46:04 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Thu, 21 Apr 2022 03:47:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 21 Apr 2022 03:47:20 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 21 Apr 2022 03:47:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 21 Apr 2022 03:47:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 21 Apr 2022 03:47:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 21 Apr 2022 03:47:39 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 21 Apr 2022 03:47:40 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Thu, 21 Apr 2022 03:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 03:47:48 GMT
STOPSIGNAL SIGINT
# Thu, 21 Apr 2022 03:47:49 GMT
EXPOSE 5432
# Thu, 21 Apr 2022 03:47:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5e0d035960b14409a1ddb839de80aa08677b71addd5e94264ff9ee89a2523e5b`  
		Last Modified: Wed, 20 Apr 2022 09:56:59 GMT  
		Size: 35.3 MB (35285249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c5c9eed70514d1994a21525f0ddaa949a3bfa0cef33a61e1a32bc6bf27d60a`  
		Last Modified: Thu, 21 Apr 2022 03:58:44 GMT  
		Size: 5.2 MB (5223060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898e2dab6f2cd3cb6cfcf05ea00e2ef06c2e73c79ab8a81c1180cae2dae52257`  
		Last Modified: Thu, 21 Apr 2022 03:58:42 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7094ea53f38e12bc7bd21096f870e0a78ae4739e21f338b62b0a1de776c6885`  
		Last Modified: Thu, 21 Apr 2022 03:58:41 GMT  
		Size: 1.3 MB (1317628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e5cca229ebb5fe10a9b095018558e5c5cbc2aac3997202d3a1630e41447ff3`  
		Last Modified: Thu, 21 Apr 2022 03:58:41 GMT  
		Size: 8.0 MB (8045576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da288b0b75b4cf267391138b7d84164632bb00e16dc819c3494183bf292e1e72`  
		Last Modified: Thu, 21 Apr 2022 03:58:40 GMT  
		Size: 1.4 MB (1420301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd6ccc8042ac0819b98b584d1a82e07c7b980e1057a7734da2e0c2019729715`  
		Last Modified: Thu, 21 Apr 2022 03:58:39 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ad7407b3190e6d4a78fefe2be75b984a26b2e31ae2672d20c091b7017e869a`  
		Last Modified: Thu, 21 Apr 2022 03:58:38 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c8136358e321e5a351b03913ea2a1c0eacacccb0f55871717b07fa6ec09837`  
		Last Modified: Thu, 21 Apr 2022 03:58:52 GMT  
		Size: 95.6 MB (95581753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf29518b890046fb8847d6ea0cf79cfcba6506e633eb0b89d0efdafcc825597a`  
		Last Modified: Thu, 21 Apr 2022 03:58:35 GMT  
		Size: 9.5 KB (9533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d25814ea98da8e0eeb4c02ab4e76a58a401b33fc6d04758ccaf98a4c9c6a81f`  
		Last Modified: Thu, 21 Apr 2022 03:58:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f95fbeeed1bb9185581104331b65eaabdd7a3ecd1b2cd78dee23c213f62145`  
		Last Modified: Thu, 21 Apr 2022 03:58:35 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dbfd9cf0b39a1ab3e062efb4c747452b73bfc8e0db1cb5264084126b20077b`  
		Last Modified: Thu, 21 Apr 2022 03:58:35 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; s390x

```console
$ docker pull postgres@sha256:6ac10ee1fafb76c56c76dbfc452a477e076425ecdfdf22d4f620ac4e45e259cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85130463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a53291a87d6d9e795661376225168c6e62645b6306f37fd290fb24fc2bee1c15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Apr 2022 08:39:37 GMT
ADD file:c3381330644d6d9fc585301395580b564cdf7c880fb2dc2d8e48992673184f7d in / 
# Wed, 20 Apr 2022 08:39:42 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:04:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 20:04:49 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 20 Apr 2022 20:04:49 GMT
ENV GOSU_VERSION=1.14
# Wed, 20 Apr 2022 20:04:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 20 Apr 2022 20:05:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 20 Apr 2022 20:05:05 GMT
ENV LANG=en_US.utf8
# Wed, 20 Apr 2022 20:05:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:05:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 20 Apr 2022 20:05:11 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 20 Apr 2022 20:05:11 GMT
ENV PG_MAJOR=14
# Wed, 20 Apr 2022 20:05:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Wed, 20 Apr 2022 20:05:12 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Wed, 20 Apr 2022 20:12:49 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 20 Apr 2022 20:12:51 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 20 Apr 2022 20:12:52 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 20 Apr 2022 20:12:52 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 20 Apr 2022 20:12:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 20 Apr 2022 20:12:53 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 20 Apr 2022 20:12:53 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 20 Apr 2022 20:12:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 20:12:53 GMT
STOPSIGNAL SIGINT
# Wed, 20 Apr 2022 20:12:53 GMT
EXPOSE 5432
# Wed, 20 Apr 2022 20:12:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3179e1eccb473ae22a70e8ac3e9ddb4660ebdfd977989d115bd4d322ecc12b89`  
		Last Modified: Wed, 20 Apr 2022 08:49:39 GMT  
		Size: 29.7 MB (29654805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc654ca7560676add519eccc966b27aa7d1b949a6dd5a625329d8a12085462ba`  
		Last Modified: Wed, 20 Apr 2022 20:51:33 GMT  
		Size: 4.3 MB (4302361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fc070057195088a53aa77e772340cbf5b5ec5ca0da8b56a76b086d15fd4299`  
		Last Modified: Wed, 20 Apr 2022 20:51:33 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ffb890a813f63d2ae1234d3d012524ea58d758799b26a4106572729eb31545`  
		Last Modified: Wed, 20 Apr 2022 20:51:32 GMT  
		Size: 1.4 MB (1381518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9886a8bc67ed0cbc73a0027cdc9de8bb8f0905390e23509b072ddf2eca24d980`  
		Last Modified: Wed, 20 Apr 2022 20:51:33 GMT  
		Size: 8.1 MB (8099073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7234799fb9cf38b31e56fc9334f6635639a1f701164eb2e8102490ce3b5921ec`  
		Last Modified: Wed, 20 Apr 2022 20:51:31 GMT  
		Size: 1.2 MB (1237978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa47d8d71fd5464e6dfb1e756414b4dab7963383db13f07a44412a61288cb92`  
		Last Modified: Wed, 20 Apr 2022 20:51:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aae76e8fca2cecaa6372cf7bfc1024255286ee7dc527686847d8ae80f1247a3`  
		Last Modified: Wed, 20 Apr 2022 20:51:31 GMT  
		Size: 3.2 KB (3193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14aef4d26f63e7d485246659c8b40171e35b62bafa1c6f6b5769893d013cf44f`  
		Last Modified: Wed, 20 Apr 2022 20:51:35 GMT  
		Size: 40.4 MB (40435014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058ddc42e6922bb463e2b9adb5fb019fa459b65bdcf6afd138c30ccd20680c2e`  
		Last Modified: Wed, 20 Apr 2022 20:51:29 GMT  
		Size: 9.5 KB (9540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c520a1d221166c35236a16b26062359f2ae325e15c32866e121b57a2ef78ab`  
		Last Modified: Wed, 20 Apr 2022 20:51:30 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc47cfae1738830600365d2546033816b30b5949c9731322fdb37658a0669c4`  
		Last Modified: Wed, 20 Apr 2022 20:51:30 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7396cfecbb7e3f1cff426c761f8375d0c7409b2bcbb8ba0f629523f1ab75f817`  
		Last Modified: Wed, 20 Apr 2022 20:51:29 GMT  
		Size: 4.7 KB (4698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
