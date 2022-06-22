## `postgres:10-stretch`

```console
$ docker pull postgres@sha256:7147bcbf2cae1f5bfda29f4993459ef21844d4b93825ae92e3a072e538c2a949
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
$ docker pull postgres@sha256:da3b91cba76db664b56e3f07bbeb9347ebc554452fbb03814006a5c32d7b64a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74101385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b35df707a62e692e5aff0f772a3b9b853c9eee9b22fd8481165d4fa303198b99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 28 May 2022 01:22:19 GMT
ADD file:d7acabc78d998195522bc84475bc7d834e451aba4eb84f813f1eeecc4b3269d7 in / 
# Sat, 28 May 2022 01:22:20 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:52:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 11:52:50 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 28 May 2022 11:52:50 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 11:53:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 11:53:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 28 May 2022 11:53:07 GMT
ENV LANG=en_US.utf8
# Sat, 28 May 2022 11:53:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:53:12 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 11:53:15 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 11:54:14 GMT
ENV PG_MAJOR=10
# Sat, 28 May 2022 11:54:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sat, 28 May 2022 11:54:14 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Sat, 28 May 2022 11:54:29 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 28 May 2022 11:54:30 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 28 May 2022 11:54:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 May 2022 11:54:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 May 2022 11:54:31 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 May 2022 11:54:31 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 22 Jun 2022 01:43:25 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Wed, 22 Jun 2022 01:43:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 22 Jun 2022 01:43:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jun 2022 01:43:26 GMT
STOPSIGNAL SIGINT
# Wed, 22 Jun 2022 01:43:26 GMT
EXPOSE 5432
# Wed, 22 Jun 2022 01:43:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:73e8e05762864dd5f0a339ca8471e27294d125b63c8adfb278e84c105b8c842d`  
		Last Modified: Sat, 28 May 2022 01:29:04 GMT  
		Size: 22.6 MB (22567519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd2c791c615587f433db1fcbb6cb3c84f974c5fdc164c1dc074a2edaad49243`  
		Last Modified: Sat, 28 May 2022 11:57:57 GMT  
		Size: 4.5 MB (4504004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032ff93c63c9508452dd82a343c8a7dff818352a18ed5c2d9573008dcd50da08`  
		Last Modified: Sat, 28 May 2022 11:57:56 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42b841ca8a1e92189abcff12b63291f466b507a3fb5669e379a59ff1d259338`  
		Last Modified: Sat, 28 May 2022 11:57:56 GMT  
		Size: 1.4 MB (1379542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5593d63858bdc24581ea5979a0670683d945a5e5e67be61393147d05325ca0f0`  
		Last Modified: Sat, 28 May 2022 11:57:55 GMT  
		Size: 6.2 MB (6185548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f6dcca2350c10616cf6f59723b3f1a040057f6dcc9436664185ea054d9d8c5`  
		Last Modified: Sat, 28 May 2022 11:57:54 GMT  
		Size: 1.2 MB (1249919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acbd90096491bfd5d1912721dfe7441387f64ac24637ee41a9ce783d4ba35c7`  
		Last Modified: Sat, 28 May 2022 11:57:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67283591ee446b8d9333ec338ae497a05c121b79e27ea179a2aa1218e4d32ff7`  
		Last Modified: Sat, 28 May 2022 11:57:54 GMT  
		Size: 5.6 KB (5584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef58b7f9fd7ec50f7191a6b7fe7e02e1d5168f17773e20a957630941242c8ff5`  
		Last Modified: Sat, 28 May 2022 11:58:51 GMT  
		Size: 38.2 MB (38194086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b56caa8e087d2f1c5fb0bb1ec989308e5184746fefd29978d9d7b7a73f73a8f`  
		Last Modified: Sat, 28 May 2022 11:58:40 GMT  
		Size: 8.1 KB (8073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac7a59ff492c569de36fe1a70bc105ab879a7fd182ff0f3a66b204650a7dd28`  
		Last Modified: Sat, 28 May 2022 11:58:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736430f8154907d0a41a3e1d0122c2676de46802980915415101bbd223c7f021`  
		Last Modified: Sat, 28 May 2022 11:58:40 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d42b33e809d87cc70b523739b108903ec977b6ab87713e89bc88c27913c58f`  
		Last Modified: Wed, 22 Jun 2022 01:47:42 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2e6f0205eae1fcbbc442978d941222ba4f34c646719830b393556b11081eb9`  
		Last Modified: Wed, 22 Jun 2022 01:47:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:9aeaaca558b8ed118fe91c811e01f43e31aa94c6047e834327c6a190492195b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71089820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f539af21c8d4bd40c6e7cebe6989f826a72ea7ae6c198290fa2166d7dfcff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 28 May 2022 02:08:55 GMT
ADD file:483f9abf6a9bfe57925361419f3c33378ea0de816efd7fa9061c5d865b84698f in / 
# Sat, 28 May 2022 02:08:55 GMT
CMD ["bash"]
# Sun, 29 May 2022 03:34:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 03:34:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 29 May 2022 03:34:31 GMT
ENV GOSU_VERSION=1.14
# Sun, 29 May 2022 03:35:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 29 May 2022 03:35:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 29 May 2022 03:35:23 GMT
ENV LANG=en_US.utf8
# Sun, 29 May 2022 03:35:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 03:35:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 29 May 2022 03:35:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sun, 29 May 2022 04:26:30 GMT
ENV PG_MAJOR=10
# Sun, 29 May 2022 04:26:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sun, 29 May 2022 04:26:30 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Sun, 29 May 2022 04:52:57 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sun, 29 May 2022 04:52:59 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 29 May 2022 04:53:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 29 May 2022 04:53:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 29 May 2022 04:53:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 29 May 2022 04:53:04 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 22 Jun 2022 00:29:29 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Wed, 22 Jun 2022 00:29:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 22 Jun 2022 00:29:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jun 2022 00:29:31 GMT
STOPSIGNAL SIGINT
# Wed, 22 Jun 2022 00:29:31 GMT
EXPOSE 5432
# Wed, 22 Jun 2022 00:29:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:79d5abb6d30cb3b0229b118def5c682e5bc6cedb38ed44f4ad517b8310316288`  
		Last Modified: Sat, 28 May 2022 02:26:04 GMT  
		Size: 21.2 MB (21240746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfce0a17747ca78978225d06a1a8acbb9c829b0b87465e7c0b824ebdb37a7d0c`  
		Last Modified: Sun, 29 May 2022 05:01:45 GMT  
		Size: 4.2 MB (4239517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656582b77844ac5457e657bebcc8249842dd997e3c2570f1c0198218c03ca3b1`  
		Last Modified: Sun, 29 May 2022 05:01:41 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c1f18b5b555e428889a9d0e8303ca01b7b94a5514b825c25da209f6f961bad`  
		Last Modified: Sun, 29 May 2022 05:01:42 GMT  
		Size: 1.3 MB (1344490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6941fb7729ff3ef656c9ac61b7c468d3b1e032568bfe78b98c74fdb8ef629c`  
		Last Modified: Sun, 29 May 2022 05:01:44 GMT  
		Size: 6.2 MB (6185871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c7f7559a297b3a7df87f5faf1cfd520228d6afc90484ea07b51ae5b1aad6d0`  
		Last Modified: Sun, 29 May 2022 05:01:40 GMT  
		Size: 1.2 MB (1194846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c548a9bc74ce778282ae481c88a604e10adb406b63e5b7797ac8c53855c1940d`  
		Last Modified: Sun, 29 May 2022 05:01:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ab71a24e4141a4cb5db7425b419ca0826cbb9ddb9a2a80dbadfd6118bbdf90`  
		Last Modified: Sun, 29 May 2022 05:01:40 GMT  
		Size: 5.6 KB (5584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0803ae069d414bda2b8b0b55fd18a33264df40f5b52058696c30d37d7318b78`  
		Last Modified: Sun, 29 May 2022 05:03:26 GMT  
		Size: 36.9 MB (36863575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81142be1e9e2e5d2408d6508bd71ab89bd1aebb8912486203ad4011f676186a4`  
		Last Modified: Sun, 29 May 2022 05:03:02 GMT  
		Size: 8.1 KB (8081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab7be939b175bd2c15e6c3dd73feb49d9438334c5bcc67e3fa16f561954cd6`  
		Last Modified: Sun, 29 May 2022 05:03:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a692eb7973060032bf40ebe0297815643c1beebac52e0883136d62188637e902`  
		Last Modified: Sun, 29 May 2022 05:03:02 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0464e7550cccb89ad87c4275f763ddd42d68462e7b3bedcef369d25af84e70fe`  
		Last Modified: Wed, 22 Jun 2022 00:34:42 GMT  
		Size: 4.7 KB (4711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dccd8453460e601e7dc43814b95eab04155967a7ae3555742dc6f4354028314`  
		Last Modified: Wed, 22 Jun 2022 00:34:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:e1a9051dd7b419c17a904fc3e66ce5cbc778a69457d9e69d65f5a7100a135712
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67681233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711701b7c19df84bbbe60d6aee92ec6826bd8ec5bd208e720aee8fa02ebe9fd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 28 May 2022 01:05:51 GMT
ADD file:4dd5baef6913cbeaba8b4abeb9fa3860736e9c421334170bf9a435f002176781 in / 
# Sat, 28 May 2022 01:05:52 GMT
CMD ["bash"]
# Sun, 29 May 2022 13:53:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 29 May 2022 13:53:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sun, 29 May 2022 13:53:23 GMT
ENV GOSU_VERSION=1.14
# Sun, 29 May 2022 13:53:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sun, 29 May 2022 13:54:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sun, 29 May 2022 13:54:06 GMT
ENV LANG=en_US.utf8
# Sun, 29 May 2022 13:54:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 13:54:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sun, 29 May 2022 13:54:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sun, 29 May 2022 14:40:42 GMT
ENV PG_MAJOR=10
# Sun, 29 May 2022 14:40:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sun, 29 May 2022 14:40:43 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Sun, 29 May 2022 15:04:01 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sun, 29 May 2022 15:04:03 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sun, 29 May 2022 15:04:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sun, 29 May 2022 15:04:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sun, 29 May 2022 15:04:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sun, 29 May 2022 15:04:07 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 22 Jun 2022 00:42:03 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Wed, 22 Jun 2022 00:42:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 22 Jun 2022 00:42:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jun 2022 00:42:05 GMT
STOPSIGNAL SIGINT
# Wed, 22 Jun 2022 00:42:06 GMT
EXPOSE 5432
# Wed, 22 Jun 2022 00:42:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b1bc9eb7248815be774e7f369470fa41493ff76db8a85f10e545b1538909d9d7`  
		Last Modified: Sat, 28 May 2022 01:22:13 GMT  
		Size: 19.4 MB (19359814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46abaac493e789a2c0689959997f3b2652cc64c7c005995d1af3fc2d9808ec2`  
		Last Modified: Sun, 29 May 2022 15:14:36 GMT  
		Size: 3.9 MB (3875664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d246ac12943b16438b10323b5e2feba727c48121af4ae5c618d288c0c4debb06`  
		Last Modified: Sun, 29 May 2022 15:14:34 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69279ed0aa6c34fe0ad54bafe82f1016d3d8241b980e6044ed697b4c57fe877`  
		Last Modified: Sun, 29 May 2022 15:14:35 GMT  
		Size: 1.3 MB (1336052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f86c79ccf150dd0cf33bf549d883999cad9340e2cc1f3d43ffddb4225c6d021`  
		Last Modified: Sun, 29 May 2022 15:14:36 GMT  
		Size: 6.2 MB (6185877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8d5f0cb1f2ae00aea41959e9af1ec016c27af7459a004903f94163cd8503c2`  
		Last Modified: Sun, 29 May 2022 15:14:33 GMT  
		Size: 1.1 MB (1097056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b78f7b73d4c6b8f13b0c47e12adf526bbe20937e851e86fa72febadafaf389`  
		Last Modified: Sun, 29 May 2022 15:14:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfcf7160440c0eb4b7f03b23043287439d0694a7c73191f0d6b7ffa67e32981`  
		Last Modified: Sun, 29 May 2022 15:14:32 GMT  
		Size: 5.6 KB (5585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020a700bb1847c9fd382a38125f6ddd37b5fb4187a668c802855557c9b4229bc`  
		Last Modified: Sun, 29 May 2022 15:16:21 GMT  
		Size: 35.8 MB (35805991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110d4f6231b7f10f5767ba23b7641b019af6ab341fdde94ca1cdaed4f77a6823`  
		Last Modified: Sun, 29 May 2022 15:15:57 GMT  
		Size: 8.1 KB (8079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d6141f9f4021dbfdf4dbdfde6bba2e125cc1715067aaea0addbe7872049f23`  
		Last Modified: Sun, 29 May 2022 15:15:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7875aab2d87ca276d6cb2ac1dbe3fcbe4567159183f900ff995df6342d676567`  
		Last Modified: Sun, 29 May 2022 15:15:57 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5fabe00016fb85883fcdbd59371721795633196f33f720afec43db40565597`  
		Last Modified: Wed, 22 Jun 2022 00:51:33 GMT  
		Size: 4.7 KB (4711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6788b708615a0a3bfdd15c630b087ff0a77a11d30e396431bdf9dde26045ae4`  
		Last Modified: Wed, 22 Jun 2022 00:51:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:826e136b95290848c7cff8e3fd2d7642278f5fe76f11c09db178b5d366ac4890
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.0 MB (69985590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f579ed3acd9b4991e97c2f8e74feccd551a2c38516dea599781408b1baecb938`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 28 May 2022 00:43:00 GMT
ADD file:5d3acfb1c09652c954868b7e7fba2e995e5e143bd0f2b1c04a34897232913f7a in / 
# Sat, 28 May 2022 00:43:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 06:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 06:50:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 28 May 2022 06:50:54 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 06:51:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 06:51:12 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 28 May 2022 06:51:13 GMT
ENV LANG=en_US.utf8
# Sat, 28 May 2022 06:51:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 06:51:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 06:51:23 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 07:01:44 GMT
ENV PG_MAJOR=10
# Sat, 28 May 2022 07:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sat, 28 May 2022 07:01:46 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Sat, 28 May 2022 07:11:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 28 May 2022 07:11:24 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 28 May 2022 07:11:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 May 2022 07:11:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 May 2022 07:11:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 May 2022 07:11:27 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 28 May 2022 07:11:29 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Sat, 28 May 2022 07:11:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 28 May 2022 07:11:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 07:11:31 GMT
STOPSIGNAL SIGINT
# Sat, 28 May 2022 07:11:32 GMT
EXPOSE 5432
# Sat, 28 May 2022 07:11:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5787d8ce843947b58d50c514418ca92eca29e2110be4fe2993451d835d2d846a`  
		Last Modified: Sat, 28 May 2022 00:51:48 GMT  
		Size: 20.4 MB (20424104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b17ea5d1e741473a39b1a7e5eca5a742b930d73b147217ddaa7bbe347e4aaca`  
		Last Modified: Sat, 28 May 2022 07:16:07 GMT  
		Size: 3.9 MB (3890932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497e293642c352f67b7637126f4eea8b184eb608cf50d376d8a2985c853980d`  
		Last Modified: Sat, 28 May 2022 07:16:06 GMT  
		Size: 1.7 KB (1664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e99dbea293843ebcdf20ea4843c630325366f7f864665a3d1b71234b6f7a9a`  
		Last Modified: Sat, 28 May 2022 07:16:06 GMT  
		Size: 1.3 MB (1307859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09579ff3ea4da0bf8dd6881242db63a6eddf4994c794b4fa8cb07b22cb8ed281`  
		Last Modified: Sat, 28 May 2022 07:16:05 GMT  
		Size: 6.2 MB (6182574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dac6704479db1d6858a29da897365a51f12e23c655fdf8c3528db64a4dc270`  
		Last Modified: Sat, 28 May 2022 07:16:04 GMT  
		Size: 1.0 MB (1007478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9db756532cf3958282c4f6c52e9f0d8cc19a4ecda8d91ed30b3005744fb8473`  
		Last Modified: Sat, 28 May 2022 07:16:03 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed841cf8dfd2b92969f717e0e33d51f953a8837187b05edbb84312ebe6ecd43`  
		Last Modified: Sat, 28 May 2022 07:16:03 GMT  
		Size: 5.5 KB (5525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8aba4bb7a7c6f33554488852d50dad4a4eb67eabd0b3be89bd7c4b0c22de8d0`  
		Last Modified: Sat, 28 May 2022 07:16:57 GMT  
		Size: 37.2 MB (37152139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02222bad3091c57650545e3dc81b6278ea40feb146ce6e58bacad6ae80935c`  
		Last Modified: Sat, 28 May 2022 07:16:49 GMT  
		Size: 8.1 KB (8077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3735a732b755c42ef4f5c228062ad83affa852677a047ef706286c947d2aee`  
		Last Modified: Sat, 28 May 2022 07:16:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358615225b5b9c85c94a2d9efb4689a96fd75edca8c26590390fa55e0819009e`  
		Last Modified: Sat, 28 May 2022 07:16:49 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3a7c3c02f5fd24737a5cc2d864cc0e2a3b34d1791fbba4733780d0c7480988`  
		Last Modified: Sat, 28 May 2022 07:16:49 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ba9d5e8d445b554b2f0447dcc6f23720ab665909191d11e8238ade58581116`  
		Last Modified: Sat, 28 May 2022 07:16:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-stretch` - linux; 386

```console
$ docker pull postgres@sha256:b8a9d90afdd3ac489f83c0263fde1cd84f93c5b2fa7d9ee5a1c667e3a95f0568
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.9 MB (74852497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87d5585824e7e354b211aa2e963c97991112b214a75c10d36f3ba260a1ddf257`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Sat, 28 May 2022 00:42:06 GMT
ADD file:6293189b62f79ff468fca4fbbfa2c9feeb7dbde24f78e75aba7519eea5a057c0 in / 
# Sat, 28 May 2022 00:42:06 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:25:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 07:25:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 28 May 2022 07:25:53 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 07:26:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 07:26:11 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 28 May 2022 07:26:12 GMT
ENV LANG=en_US.utf8
# Sat, 28 May 2022 07:26:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:26:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 28 May 2022 07:26:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 28 May 2022 07:36:18 GMT
ENV PG_MAJOR=10
# Sat, 28 May 2022 07:36:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Sat, 28 May 2022 07:36:19 GMT
ENV PG_VERSION=10.21-1.pgdg90+1
# Sat, 28 May 2022 07:36:35 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 28 May 2022 07:36:36 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 28 May 2022 07:36:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 28 May 2022 07:36:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 28 May 2022 07:36:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 28 May 2022 07:36:40 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 22 Jun 2022 02:01:00 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Wed, 22 Jun 2022 02:01:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 22 Jun 2022 02:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:01:02 GMT
STOPSIGNAL SIGINT
# Wed, 22 Jun 2022 02:01:03 GMT
EXPOSE 5432
# Wed, 22 Jun 2022 02:01:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b40cd57a2ae5df70065f52d290f1d458989047a30430e8c08ff459364faefda0`  
		Last Modified: Sat, 28 May 2022 00:50:56 GMT  
		Size: 23.2 MB (23202396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85041cc10669ef26bad946cd70aad0bc328f612c0ac45abf25c54609fa81ea99`  
		Last Modified: Sat, 28 May 2022 07:41:20 GMT  
		Size: 4.6 MB (4623938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7283f314b49e80dc5dc0dd7ac7a4f8ec95a0edc7ffdd78e2f145f0a007fb8488`  
		Last Modified: Sat, 28 May 2022 07:41:19 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e9daf8073e426fee1f9d7e6609af6df0ca9f2a148ec23e0252e6da40061dda`  
		Last Modified: Sat, 28 May 2022 07:41:19 GMT  
		Size: 1.3 MB (1346983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d93421df4b574d729ee9114cfc8363d2e6b820e60e3ec25ab34a82454c5d6d3`  
		Last Modified: Sat, 28 May 2022 07:41:18 GMT  
		Size: 6.2 MB (6182823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6264e9a5b339409a0b9638e9a11fceb70c5cfe6c59cbf453336dd2b6427cc8`  
		Last Modified: Sat, 28 May 2022 07:41:17 GMT  
		Size: 1.0 MB (1030569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f37e4674d2d6174b0cf2e09cfdd6b67d91969b529155e698569d92d55e3cd8b`  
		Last Modified: Sat, 28 May 2022 07:41:16 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b3cf0c0727ed283d5acf593dec942a4b65382dd91b0e089dbb8efeafe883b0`  
		Last Modified: Sat, 28 May 2022 07:41:16 GMT  
		Size: 5.5 KB (5526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f5c7ff1aaab8eedb7d75b364b7871513a62e0a35a6b74ba316c33ab9d3899b`  
		Last Modified: Sat, 28 May 2022 07:42:17 GMT  
		Size: 38.4 MB (38445290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57eaeff296e558a68c459984d70fc7214d077b7ae3ae491146418da716a924`  
		Last Modified: Sat, 28 May 2022 07:42:05 GMT  
		Size: 8.1 KB (8077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebc1896ea6501d5f930daac97678042a15e1f9bb800758e8adab345c6b588e5`  
		Last Modified: Sat, 28 May 2022 07:42:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1a372a442213fd5c2ec82eee8be4c63171d596e9a171c668485aa8b45ac660`  
		Last Modified: Sat, 28 May 2022 07:42:05 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bc7eb3c5e6f56c1786a54339d5d0d888fa007fcbe1be4dea53ad30a34de0c8`  
		Last Modified: Wed, 22 Jun 2022 02:06:50 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc99cd9371e939b4a884a974ad031ffe820f6a2ecfabee50dc411e6e5731533`  
		Last Modified: Wed, 22 Jun 2022 02:06:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
