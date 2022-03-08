## `postgres:10-stretch`

```console
$ docker pull postgres@sha256:7da30a5bf4b6a7afaf1306c4e5ee2387eb85f905f031b3da3c837b0cb4816995
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
$ docker pull postgres@sha256:2d94b740f7746173e7c9894eea9d799837ed6787a4d2374cfa07518c987b4894
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74056563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7b726c2a58082b7502e2df32a33ce09098c75fec53939e523a07c5d8c9a69f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:16:08 GMT
ADD file:81245cad973855905213c6025084b80656d9513a3611781ea4150d76705aa1c6 in / 
# Tue, 01 Mar 2022 02:16:08 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 01:32:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Mar 2022 01:32:05 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 02 Mar 2022 01:32:06 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Mar 2022 01:32:18 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Mar 2022 01:32:23 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 02 Mar 2022 01:32:23 GMT
ENV LANG=en_US.utf8
# Tue, 08 Mar 2022 19:53:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Mar 2022 19:53:50 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 08 Mar 2022 19:54:23 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 08 Mar 2022 20:01:11 GMT
ENV PG_MAJOR=10
# Tue, 08 Mar 2022 20:01:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 08 Mar 2022 20:01:11 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Tue, 08 Mar 2022 20:01:26 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 08 Mar 2022 20:01:26 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:01:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:01:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:01:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:01:28 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:01:28 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:01:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 08 Mar 2022 20:01:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:01:29 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:01:29 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:01:29 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:93830f6d38936ace1b18d4bf04c82ba5177c67672db5610604596fd46f6e9c18`  
		Last Modified: Tue, 01 Mar 2022 02:23:11 GMT  
		Size: 22.5 MB (22529127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4647eccb1aeb9c8705a69482d899afa962c0d1eaefdda2e9b1ec284c4dd27e`  
		Last Modified: Wed, 02 Mar 2022 01:38:11 GMT  
		Size: 4.5 MB (4503855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a3cee4f6bdad09e61e235b8492d80f18f12db25234ca95e6d1bec165edbbbc`  
		Last Modified: Wed, 02 Mar 2022 01:38:09 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206ea0712d22fbec684e4e486a9976a5729889033e354e4c65e57311df8a352d`  
		Last Modified: Wed, 02 Mar 2022 01:38:10 GMT  
		Size: 1.4 MB (1379343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e29d016784a3662f18c95d93901d1b8f9f53691990e018490cf2cd730cd044f`  
		Last Modified: Wed, 02 Mar 2022 01:38:08 GMT  
		Size: 6.2 MB (6185423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0ae6aeb77550fa14e2bb63288da85ade3ef5930d3342f08b2fbb338eb1bf54`  
		Last Modified: Tue, 08 Mar 2022 20:10:34 GMT  
		Size: 1.2 MB (1249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb32f91fc7fea43c9c45d7c32ffdd98a3194e721ed843d6d5da8135e9089b7fb`  
		Last Modified: Tue, 08 Mar 2022 20:10:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3021590b2d1012de86af1102050ddfef5828f00691700f6bb50954b149c515`  
		Last Modified: Tue, 08 Mar 2022 20:10:34 GMT  
		Size: 5.6 KB (5589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7a2735e92208ded9e202355c9a903bf8f5ad42e4d9ba7dfae5336b8d6100ca`  
		Last Modified: Tue, 08 Mar 2022 20:12:00 GMT  
		Size: 38.2 MB (38188302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10de428821245b481441794af9a75b01f536a0e39b36ffa1fe6cb65318c4884`  
		Last Modified: Tue, 08 Mar 2022 20:11:50 GMT  
		Size: 8.1 KB (8073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ce2e8e01f486618405849d1f90f3783a2decfe232746a485eb3cb0595fc2ed`  
		Last Modified: Tue, 08 Mar 2022 20:11:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8b074874ea0f2d6b07b079f81bae123a16a11952b4cb57f2471c8c54ce2355`  
		Last Modified: Tue, 08 Mar 2022 20:11:50 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7bc434cc89f2129ec846852fceb8fe15055ae40ae548e1a95ff28d1405231`  
		Last Modified: Tue, 08 Mar 2022 20:11:50 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0eb00bc4f47234c9ab2c80ab141328b603049fbc6eddb90a7ecb2df7cb8747`  
		Last Modified: Tue, 08 Mar 2022 20:11:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:a7a971e6bcaa10fa9dc249b69245be98dc05dee528d3a7223ab5843a8dfa0d52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70234508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e09e9f4de86069423e87ec85659366c47808ddf23eb073ca13e9cd9e0d27627`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:47 GMT
ADD file:7ba67de2da2d36a62cc2408396fc8c8571ddec0f9e54398459b261e0ce1f73f2 in / 
# Tue, 01 Mar 2022 02:08:48 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 11:49:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 11:49:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 01 Mar 2022 11:49:22 GMT
ENV GOSU_VERSION=1.14
# Tue, 01 Mar 2022 11:49:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 01 Mar 2022 11:50:13 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 01 Mar 2022 11:50:13 GMT
ENV LANG=en_US.utf8
# Tue, 01 Mar 2022 11:50:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 11:50:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 01 Mar 2022 11:50:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 01 Mar 2022 12:41:18 GMT
ENV PG_MAJOR=10
# Tue, 01 Mar 2022 12:41:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 01 Mar 2022 12:41:18 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Tue, 01 Mar 2022 13:07:24 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 01 Mar 2022 13:07:27 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 01 Mar 2022 13:07:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 01 Mar 2022 13:07:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 01 Mar 2022 13:07:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 01 Mar 2022 13:07:32 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 01 Mar 2022 13:07:32 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Tue, 01 Mar 2022 13:07:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 01 Mar 2022 13:07:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 13:07:35 GMT
STOPSIGNAL SIGINT
# Tue, 01 Mar 2022 13:07:35 GMT
EXPOSE 5432
# Tue, 01 Mar 2022 13:07:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e1fc40b579c554284072c098e17ce2034889200a36f1168e6e6baed4aab3de88`  
		Last Modified: Tue, 01 Mar 2022 02:26:15 GMT  
		Size: 21.2 MB (21203497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c689fb7ed4fdeb91555c0b99fc82eff808b671328b2d7c193c9acbd86cd6bd`  
		Last Modified: Tue, 01 Mar 2022 13:14:42 GMT  
		Size: 4.2 MB (4239326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d64d4f1e21cceae6a9fc597346f378615938e862918cccde533bfd2e6ea80b1`  
		Last Modified: Tue, 01 Mar 2022 13:14:39 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e9e26bdff95dce3f564a6205ba99fb9badd4998a74d58ae90ad2d0538be1ee`  
		Last Modified: Tue, 01 Mar 2022 13:14:39 GMT  
		Size: 1.3 MB (1344213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17883ce8a8be20fbf3d79222d5204641c7c3af1f5c566a6ecd2c4659e44fbc9f`  
		Last Modified: Tue, 01 Mar 2022 13:14:42 GMT  
		Size: 6.2 MB (6185706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b34dd189586a8519479d842cc5f10718624c106ebd9a8e029a8083f7f10de0`  
		Last Modified: Tue, 01 Mar 2022 13:14:38 GMT  
		Size: 385.0 KB (385040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1eee84502d565effc8bfb84dc369cd72b6aa0ce4a3b6d05a3d00edbab933af`  
		Last Modified: Tue, 01 Mar 2022 13:14:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713463f797a80095c136cab9f4744032898890aee3897bb132d72bbe4fa18738`  
		Last Modified: Tue, 01 Mar 2022 13:14:37 GMT  
		Size: 5.6 KB (5583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41bc2264587277685e7809279f2093dca4613d5165be4c33facb141758f0389`  
		Last Modified: Tue, 01 Mar 2022 13:16:32 GMT  
		Size: 36.9 MB (36855982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ee24bd96ae094f5b8534d17783bf5ae9f0fb96fa22c7b4f4b414ce3b65f6f5`  
		Last Modified: Tue, 01 Mar 2022 13:16:05 GMT  
		Size: 8.1 KB (8075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bde7f54b595d830ce444e3cf04593054349015be662265c7156123904cb0f2`  
		Last Modified: Tue, 01 Mar 2022 13:16:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca466af1aa1780681f431c23ed4e95eebcdb91c482190f044c76fdfcb9d1f51`  
		Last Modified: Tue, 01 Mar 2022 13:16:05 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c967faaf7c51e0e06616c26aaa40affa6207bc954c4af666864088bd4ebecd8f`  
		Last Modified: Tue, 01 Mar 2022 13:16:05 GMT  
		Size: 4.7 KB (4686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e53e3c5785bc0c8f0fcd3c21834dd9ed87ff8678539c45001a2501d656de12`  
		Last Modified: Tue, 01 Mar 2022 13:16:05 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:002aa8e4ff95c644efdf0a4ee3c2a18cebb1be52f5f932f490d25f6f5ca7653e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66911706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b1aadeaf7bcdc0d3d3bf813b85a1746da07cb5ba70839b2ee9c0804c0dcf7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:29 GMT
ADD file:b573bfb75b0df3ee547a99ec724d80518fbba40b260dadfe30467b24057bb391 in / 
# Tue, 01 Mar 2022 02:09:30 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 15:19:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Mar 2022 15:19:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 02 Mar 2022 15:19:14 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Mar 2022 15:19:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Mar 2022 15:20:00 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 02 Mar 2022 15:20:00 GMT
ENV LANG=en_US.utf8
# Wed, 02 Mar 2022 15:20:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 15:20:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 02 Mar 2022 15:43:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 02 Mar 2022 15:43:46 GMT
ENV PG_MAJOR=10
# Wed, 02 Mar 2022 15:43:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Wed, 02 Mar 2022 15:43:47 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Wed, 02 Mar 2022 16:06:58 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 02 Mar 2022 16:07:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 02 Mar 2022 16:07:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 02 Mar 2022 16:07:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 02 Mar 2022 16:07:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 02 Mar 2022 16:07:04 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 02 Mar 2022 16:07:04 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Wed, 02 Mar 2022 16:07:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 02 Mar 2022 16:07:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Mar 2022 16:07:06 GMT
STOPSIGNAL SIGINT
# Wed, 02 Mar 2022 16:07:07 GMT
EXPOSE 5432
# Wed, 02 Mar 2022 16:07:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:52aa216cc1f7f3b5d4ed3b10d96ffe1a02174398f1c9377415eb8bb643cb1782`  
		Last Modified: Tue, 01 Mar 2022 02:26:16 GMT  
		Size: 19.3 MB (19318791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8fff78517566eb7389510f5302c5b7add02e4c766a8f9af1cbea365a4cec67`  
		Last Modified: Wed, 02 Mar 2022 16:16:49 GMT  
		Size: 3.9 MB (3875486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b34b973ff1b958e76251b87eb8def1617d8611359a44c994e153a59bc3e1f7c`  
		Last Modified: Wed, 02 Mar 2022 16:16:46 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91dae5d27c36695293a83704fd411191079ee27da8cbff5986934bcb5c2710d`  
		Last Modified: Wed, 02 Mar 2022 16:16:47 GMT  
		Size: 1.3 MB (1335868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9689483ac3423bc4b415bf69cb2e879ed7b3c6436f13c4b036fe3641c0be7a`  
		Last Modified: Wed, 02 Mar 2022 16:16:49 GMT  
		Size: 6.2 MB (6185597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7bc2f1d41b33533079a53ef480790740fbd0e12071e3a758f52c8c646c89fb`  
		Last Modified: Wed, 02 Mar 2022 16:16:45 GMT  
		Size: 379.2 KB (379156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001d9ee6088e80fb085218ba1a0518fde4ab67a69e4990eb439b28695b9eafdb`  
		Last Modified: Wed, 02 Mar 2022 16:16:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0214c13af97090dfc0526e8e6fcb68d20ce9287e335c1461e0caf0f49ed13b0e`  
		Last Modified: Wed, 02 Mar 2022 16:16:44 GMT  
		Size: 5.6 KB (5585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bad538b2d4024aaffdc14fc96e388e3af572f45aa44af6d3f85f31d125061d5`  
		Last Modified: Wed, 02 Mar 2022 16:17:08 GMT  
		Size: 35.8 MB (35796063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ced8fa1e9592f5ba507794ca29b2d9f498e45ab46424fbcc784c0b754c40a4`  
		Last Modified: Wed, 02 Mar 2022 16:16:43 GMT  
		Size: 8.1 KB (8075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5811861ae1c6b53670bd73f6754949bc3865bb21caeea9eb83bb8056939d1fc9`  
		Last Modified: Wed, 02 Mar 2022 16:16:43 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3773d940c973ad3d4f27e30d5725d2c4e9704dfe8a2b42e64221a0f2f814c6cb`  
		Last Modified: Wed, 02 Mar 2022 16:16:43 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b707cbcbfa18a418fdf2c78c4efd6c0b8dd7247437a17a29da76e4db1217a5a0`  
		Last Modified: Wed, 02 Mar 2022 16:16:43 GMT  
		Size: 4.7 KB (4688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ffed80f72b01c2a5f48b4a723f0fe34ddc1400341c621a76619baad1bdd8df`  
		Last Modified: Wed, 02 Mar 2022 16:16:43 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:d029968a9c78a042cac928b1909d3b84dd97f950540ca70bf0ae3dc10721bd38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69945360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76699c257613b25d2bf77c3110f65ad766cc3f3126c542a87449b05e6a07de7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:14:02 GMT
ADD file:7c0937a756dd9db418c6dc8bbb98775215961a535aa28d3940a8415bda425fda in / 
# Tue, 01 Mar 2022 02:14:03 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 18:37:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 18:38:00 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 01 Mar 2022 18:38:01 GMT
ENV GOSU_VERSION=1.14
# Tue, 01 Mar 2022 18:38:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 01 Mar 2022 18:38:20 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 01 Mar 2022 18:38:21 GMT
ENV LANG=en_US.utf8
# Tue, 08 Mar 2022 20:08:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Mar 2022 20:08:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 08 Mar 2022 20:08:47 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 08 Mar 2022 20:22:22 GMT
ENV PG_MAJOR=10
# Tue, 08 Mar 2022 20:22:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 08 Mar 2022 20:22:24 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Tue, 08 Mar 2022 20:31:13 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 08 Mar 2022 20:31:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:31:15 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:31:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:31:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:31:18 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:31:20 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:31:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 08 Mar 2022 20:31:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:31:22 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:31:23 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:31:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ccef1aa8735147c03eb756a7949a4199206181a5efe15aaf07ae3960fe5579e5`  
		Last Modified: Tue, 01 Mar 2022 02:22:40 GMT  
		Size: 20.4 MB (20389376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22db9ecffb81b1eb296a1da996499a31182d8b14bc51a7d742b7e3ff5f0cc9de`  
		Last Modified: Tue, 01 Mar 2022 19:01:58 GMT  
		Size: 3.9 MB (3890695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a76d3e580c4843799e268da42f139e919a977f6b1d0e6cf9698f0cfaeb5fda2`  
		Last Modified: Tue, 01 Mar 2022 19:01:56 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4c50dfa4a8801ecf7950c10f0b5ed5313f1ce9440e7df98e76db222ff32ddf`  
		Last Modified: Tue, 01 Mar 2022 19:01:57 GMT  
		Size: 1.3 MB (1307720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287afc666a2dec027ff38e19d9adb6d8c6249ffe383140ef12238cfc39bfd37f`  
		Last Modified: Tue, 01 Mar 2022 19:01:56 GMT  
		Size: 6.2 MB (6182384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d71b37b191f3ea939b8f08f6365a861c2bdb2fd2f89c74c92ee8dd3d80ef06`  
		Last Modified: Tue, 08 Mar 2022 20:39:26 GMT  
		Size: 1.0 MB (1007399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941b2ae28ac3fab0f564203c6d01c28552a1525df8f1e39df2bc7103841000c`  
		Last Modified: Tue, 08 Mar 2022 20:39:26 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859c495f7724f6da7a16a2235e04aa9fe984a0a1fbe0ca8fed11a5e071c72d0e`  
		Last Modified: Tue, 08 Mar 2022 20:39:26 GMT  
		Size: 5.5 KB (5530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9304ef2c1a95ded4e692d273882c189c5ceb0ce5c47463e1449799fa63a35ac9`  
		Last Modified: Tue, 08 Mar 2022 20:40:44 GMT  
		Size: 37.1 MB (37147268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6006ca0f56368d9c2356d2ae2f7fefdc708894859d8527f78cf017d43b4cac`  
		Last Modified: Tue, 08 Mar 2022 20:40:35 GMT  
		Size: 8.1 KB (8078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbad85b74295a5294b23e2bbd4a0696fb9b3a7523bf154cc91451307c83b705`  
		Last Modified: Tue, 08 Mar 2022 20:40:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699124b63b0241bef2ff179118bc8fcfb5bc59144ddde9f2fae1bf6d39a9be02`  
		Last Modified: Tue, 08 Mar 2022 20:40:35 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad709a634e78082f78bfd6aec420eaeb9803333d8fd16dcb56fb8b3604295b4f`  
		Last Modified: Tue, 08 Mar 2022 20:40:35 GMT  
		Size: 4.7 KB (4709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b105620b1680e9ad33f2572d508e9242a83869237ffbf482e107adb719e9ce62`  
		Last Modified: Tue, 08 Mar 2022 20:40:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; 386

```console
$ docker pull postgres@sha256:dbc6a6ac05103c298bdeebfe427ef614ad8a3e1db0120b7d770181c31f6e8d77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.3 MB (74349695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd5dd6353687605599df555a7d8e19dd05b59fc0f0047d21575bda7e1a08e5f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:10:29 GMT
ADD file:24ffd6980af8975d29e91cfb246c6c05f280718843056d864f5e1f4faa5a3994 in / 
# Tue, 01 Mar 2022 02:10:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 20:53:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 20:53:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 01 Mar 2022 20:53:43 GMT
ENV GOSU_VERSION=1.14
# Tue, 01 Mar 2022 20:53:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 01 Mar 2022 20:54:03 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 01 Mar 2022 20:54:03 GMT
ENV LANG=en_US.utf8
# Tue, 01 Mar 2022 20:54:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 20:54:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 01 Mar 2022 20:54:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 01 Mar 2022 21:08:29 GMT
ENV PG_MAJOR=10
# Tue, 01 Mar 2022 21:08:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Tue, 01 Mar 2022 21:08:30 GMT
ENV PG_VERSION=10.20-1.pgdg90+1
# Tue, 01 Mar 2022 21:08:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 01 Mar 2022 21:08:56 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 01 Mar 2022 21:08:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 01 Mar 2022 21:08:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 01 Mar 2022 21:08:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 01 Mar 2022 21:08:58 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 01 Mar 2022 21:08:58 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Tue, 01 Mar 2022 21:08:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 01 Mar 2022 21:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 21:08:59 GMT
STOPSIGNAL SIGINT
# Tue, 01 Mar 2022 21:08:59 GMT
EXPOSE 5432
# Tue, 01 Mar 2022 21:08:59 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:aedc5c56a757851c24982d3ca0e3be0ba560016b0d5b94c3991e01521b13e9ea`  
		Last Modified: Tue, 01 Mar 2022 02:20:42 GMT  
		Size: 23.2 MB (23157548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c7e7e74fe40501cb5529e5131642bad9ba9a943c572d28fa8124defa1d75b1`  
		Last Modified: Tue, 01 Mar 2022 21:14:41 GMT  
		Size: 4.8 MB (4812010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc0e0df46fa9d230369b6ace37c9ca820f487a9ad72504a1a9966958fadfaad`  
		Last Modified: Tue, 01 Mar 2022 21:14:40 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bdb7c9bdce2d4590bb9913e905a38dbed6563da86f800c0ee9cbcd18959f06`  
		Last Modified: Tue, 01 Mar 2022 21:14:40 GMT  
		Size: 1.3 MB (1347199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2c038502b33f877e70b8232abd1f33a7eeb2a9547fc9e123236eb56678b26b`  
		Last Modified: Tue, 01 Mar 2022 21:14:39 GMT  
		Size: 6.2 MB (6185565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3287d04f3e5ee5c64180b0b900a5e2b478d54cc66aa49eecc7db86b1d6955bc2`  
		Last Modified: Tue, 01 Mar 2022 21:14:37 GMT  
		Size: 393.3 KB (393280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eabf93b6ed8010047a530251079bf85fa6bb0dfe054c1a0d55c2e62963b7e8a`  
		Last Modified: Tue, 01 Mar 2022 21:14:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ea3cabdb30b4b704f54504ec2f6affaf91f7dc0a5d470082598d40da045f64`  
		Last Modified: Tue, 01 Mar 2022 21:14:37 GMT  
		Size: 5.6 KB (5585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ffa4940821b63cdf4cd29dbc3fdea6963e72d4e142782e4e21c8f85c38fbbc8`  
		Last Modified: Tue, 01 Mar 2022 21:15:53 GMT  
		Size: 38.4 MB (38433356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102ae8e7784d07f25a702fd575e1ef9485b824d98e34a42a818d55e43a4913b1`  
		Last Modified: Tue, 01 Mar 2022 21:15:37 GMT  
		Size: 8.1 KB (8069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519d140934b856323f5a1688ab8573a43705c443c3f3fb0638c39957eb6a0a7c`  
		Last Modified: Tue, 01 Mar 2022 21:15:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d2b5224c3d5cbbc0b3c58fb1fd4a9f52bd9960cc843764058dea312b5919bb`  
		Last Modified: Tue, 01 Mar 2022 21:15:38 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf012baee75687eaf6a7f87e8576c15fc85d89644c6b82cdc26b39e0fa687b4`  
		Last Modified: Tue, 01 Mar 2022 21:15:38 GMT  
		Size: 4.7 KB (4685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaecbc3d12ea9edb0068e63b0a5f3a3ae502fa917b0c1d64d054358cfdc92f1`  
		Last Modified: Tue, 01 Mar 2022 21:15:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
