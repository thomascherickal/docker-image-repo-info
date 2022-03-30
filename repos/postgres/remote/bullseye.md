## `postgres:bullseye`

```console
$ docker pull postgres@sha256:c97a15d76dcc7a49ccef3544e5c71fdaf27ede7716d4ec2783953e9b3520ef36
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

### `postgres:bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:1cb07b811f2ec7b7bf3c42fc3dc19c1b5e87775eee88c2b1a8793420c4de0781
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137800305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ee973e26c6564a04b427993f47091cd3ae4d5156fbd46d331b17a8e7ab45d39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 04:34:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 04:34:07 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 04:34:07 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 04:34:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 04:34:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 29 Mar 2022 04:34:22 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 04:34:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 04:34:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 04:34:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 04:34:27 GMT
ENV PG_MAJOR=14
# Tue, 29 Mar 2022 04:34:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Tue, 29 Mar 2022 04:34:27 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Tue, 29 Mar 2022 04:34:59 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 29 Mar 2022 04:35:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 04:35:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 04:35:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 04:35:01 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 04:35:01 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 04:35:01 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:35:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 04:35:02 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 04:35:02 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 04:35:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff4ca332580cb7565da7400e02683903a5b87750ea5ec6d37fe0872ce10374e`  
		Last Modified: Tue, 29 Mar 2022 05:02:18 GMT  
		Size: 4.4 MB (4414552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5037f3c12de66653b950694e1192a810bed02730e1d3c924ac8f3f1147c404dd`  
		Last Modified: Tue, 29 Mar 2022 05:02:16 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0444ef7799456c7d65fc5680240f33181ca99d3f15e9dceac5faa4b63b5bdbc4`  
		Last Modified: Tue, 29 Mar 2022 05:02:17 GMT  
		Size: 1.4 MB (1418404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47098a4166e78f44e6710c462f4f2c098c0a107ec94785144b94c038d01b11c8`  
		Last Modified: Tue, 29 Mar 2022 05:02:17 GMT  
		Size: 8.0 MB (8045338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203cca980fab7ab018cf1f99e60500f7323fbbd8b61f387adcb71fc8dc912c22`  
		Last Modified: Tue, 29 Mar 2022 05:02:15 GMT  
		Size: 1.3 MB (1260953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a479b6c0e001c21a109979efa498aba71760776b0ba9d970fa118c372650306c`  
		Last Modified: Tue, 29 Mar 2022 05:02:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa9abe8ca4e4e75ff7118c64c87b87448deb677b27064b3f4085819931aa3d`  
		Last Modified: Tue, 29 Mar 2022 05:02:14 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad613328fe382578e27c390342d33af3371c1b54907ea7d6a0575a4c814b0f3`  
		Last Modified: Tue, 29 Mar 2022 05:02:25 GMT  
		Size: 91.3 MB (91262896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce5087aacfa1dac8374b2cee6c9042ec19accb10eb4faf452bed976133049dd`  
		Last Modified: Tue, 29 Mar 2022 05:02:12 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b133d2355caa10e06dda35269c3822ed0ee4f94313d33595bdc36217a8b16645`  
		Last Modified: Tue, 29 Mar 2022 05:02:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2694eb85faff491ff29524e2861852e2d6ad2d0920a343b84b99017311b3b2e`  
		Last Modified: Tue, 29 Mar 2022 05:02:12 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503b75e1e236a9ddb637e98c72a8c3fcbe66140652a91e26990e1934d38d6ccf`  
		Last Modified: Tue, 29 Mar 2022 05:02:13 GMT  
		Size: 4.7 KB (4695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:c2d7608b32b973bfe7f70ad6fef5d5537742daf98560f3f72a8ad6ba86f42f7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131127173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0a0bfafc1fb90c5483696a887212553fc5b4ba7cb812da2ac455cc0acddb62f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 14:03:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 14:03:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 17 Mar 2022 14:03:54 GMT
ENV GOSU_VERSION=1.14
# Thu, 17 Mar 2022 14:04:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 17 Mar 2022 14:04:38 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 17 Mar 2022 14:04:39 GMT
ENV LANG=en_US.utf8
# Thu, 17 Mar 2022 14:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 14:04:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 17 Mar 2022 14:05:05 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 17 Mar 2022 14:05:05 GMT
ENV PG_MAJOR=14
# Thu, 17 Mar 2022 14:05:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 17 Mar 2022 14:05:06 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Thu, 17 Mar 2022 14:43:12 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 17 Mar 2022 14:43:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 17 Mar 2022 14:43:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 17 Mar 2022 14:43:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 17 Mar 2022 14:43:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 17 Mar 2022 14:43:18 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 17 Mar 2022 14:43:18 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Thu, 17 Mar 2022 14:43:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 14:43:19 GMT
STOPSIGNAL SIGINT
# Thu, 17 Mar 2022 14:43:20 GMT
EXPOSE 5432
# Thu, 17 Mar 2022 14:43:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44024c9d2f270ed1c396647db315fc89e66c3ca2356764e93c3cbbb9e47b76fa`  
		Last Modified: Thu, 17 Mar 2022 17:51:30 GMT  
		Size: 4.1 MB (4096461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0568f05ea2bf8332edbcbc99de05c3ffcb16a3ece32a8e0f18508759aecc3e`  
		Last Modified: Thu, 17 Mar 2022 17:51:27 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f156fc2deb637faf66d564aa065f1902efc48dcd9815f293c5ac828defa74de`  
		Last Modified: Thu, 17 Mar 2022 17:51:28 GMT  
		Size: 1.4 MB (1382544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab3c018c65715eafb6aaf547d05772c0943cbb2153574667bdb7cb7443f40a8`  
		Last Modified: Thu, 17 Mar 2022 17:51:31 GMT  
		Size: 8.0 MB (8045267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03950e2910b882c850c64e094a118c6cc45a09604fc396686cae8341e43f98f6`  
		Last Modified: Thu, 17 Mar 2022 17:51:26 GMT  
		Size: 1.3 MB (1257023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c996ba61923baa8bfb3245d14a797a0e3e41e61dd3d272332ed8a6f0c5a163b5`  
		Last Modified: Thu, 17 Mar 2022 17:51:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbdee12cae2890263f08731934032a6b1eaefa69d9536179451589ca2f30e50`  
		Last Modified: Thu, 17 Mar 2022 17:51:25 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020928dda4170fb1bee90c42b9f7897922ff29fe6cbf2e8f0543b21a1dae616a`  
		Last Modified: Thu, 17 Mar 2022 17:52:19 GMT  
		Size: 87.4 MB (87406482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d04e8c7492683f2aa7dbc99da6d69354e5d1e3a6181a4c87c779d82cc40433e`  
		Last Modified: Thu, 17 Mar 2022 17:51:24 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce1f75d401af754d8826c5eb7c673e6cb3a9858a841b815c48103769edc2515`  
		Last Modified: Thu, 17 Mar 2022 17:51:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0b552428f7e7c55e40d8e5bcb0aadadf3269d294edf4cc138003e24a651afd`  
		Last Modified: Thu, 17 Mar 2022 17:51:24 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefc704bfc00a41f044f78dce5204813cbc095acef7de03deaf48993f6764250`  
		Last Modified: Thu, 17 Mar 2022 17:51:24 GMT  
		Size: 4.7 KB (4691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:d5b954a466151d96461355a5b72581745881d4dbc4b2cdf02d8a522e2ee6d197
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125779991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30df2d12819d3597d4e031c6c362d5f228cb9252ff833ec6919ff7370a1645c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:45:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 02:45:02 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 02:45:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 02:45:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 02:45:41 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 29 Mar 2022 02:45:42 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 02:45:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 02:45:53 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 02:45:56 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 02:45:57 GMT
ENV PG_MAJOR=14
# Tue, 29 Mar 2022 02:45:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Tue, 29 Mar 2022 02:45:58 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Tue, 29 Mar 2022 03:21:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 29 Mar 2022 03:21:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 03:21:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 03:21:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 03:21:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 03:21:20 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 03:21:21 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:21:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 03:21:22 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 03:21:22 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 03:21:23 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d897fc067891a484232d4cad86253b7c9f9322409dd3f39a23f9c06ed0abd6`  
		Last Modified: Tue, 29 Mar 2022 06:36:09 GMT  
		Size: 3.7 MB (3717257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff842fa209f3f2d8445827b55c1278f364897159cd6b7e770e77bed15741be7`  
		Last Modified: Tue, 29 Mar 2022 06:36:06 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da0d8b8dad7fda7873a893caca184a12fa2b0a747005f330d29d5108068ec46`  
		Last Modified: Tue, 29 Mar 2022 06:36:07 GMT  
		Size: 1.4 MB (1375339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3715f26f891383b22ddffeaa045711a287bf66a4224e0890427a7ce34231e828`  
		Last Modified: Tue, 29 Mar 2022 06:36:11 GMT  
		Size: 8.0 MB (8045329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba370369ede33cb5556f0f429ca71873603dc77242a4d89db11d4c5f4a2e99f5`  
		Last Modified: Tue, 29 Mar 2022 06:36:05 GMT  
		Size: 1.1 MB (1131037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d025da79ab7286f8396fbe46eb62a96dc5ef716910e221c2ade3f61b0e48a4`  
		Last Modified: Tue, 29 Mar 2022 06:36:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b098075091651ed521ab833992c73474d5d4b02b877e6cbf14d83956b02c7ed1`  
		Last Modified: Tue, 29 Mar 2022 06:36:04 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420e037cdddeff135495b6dbd13fa02f3d2fb8be9f46c9d2d3b8afd1d4a416f1`  
		Last Modified: Tue, 29 Mar 2022 06:36:55 GMT  
		Size: 84.9 MB (84915954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d07e043ffffab06a940a3d81ecf455bbd8ed702d0b00e10fa8756c02ff19f76`  
		Last Modified: Tue, 29 Mar 2022 06:36:03 GMT  
		Size: 9.5 KB (9540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f950d534563ff233b4e77128de67b2f8bd7302b9786619b95e830d66c202fe8`  
		Last Modified: Tue, 29 Mar 2022 06:36:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ece937b393547128978e1ade6d81f7ae2331909759881f5cd34fe67d0d3f49`  
		Last Modified: Tue, 29 Mar 2022 06:36:03 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd32f23077c9d138326afdb79571ed3d916daca44add0a4e02aa8c58f8b0a56`  
		Last Modified: Tue, 29 Mar 2022 06:36:03 GMT  
		Size: 4.7 KB (4695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:b6dde1cdf6efe3c9f8d099b378dd79e802ef44eef164e8a662451749243f9cda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132508113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6377d4b43c303f60fcef8f34b2cc049e5c584f2e9c391de8138b4ecbf19d637f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 12:30:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 12:31:00 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 12:31:01 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 12:31:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 12:31:21 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 29 Mar 2022 12:31:22 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 12:31:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 12:31:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 12:31:30 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 12:31:31 GMT
ENV PG_MAJOR=14
# Tue, 29 Mar 2022 12:31:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Tue, 29 Mar 2022 12:31:33 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Tue, 29 Mar 2022 12:31:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 29 Mar 2022 12:31:56 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 12:31:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 12:31:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 12:31:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 12:31:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 12:32:01 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:32:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:32:02 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 12:32:03 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 12:32:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f00ab4a1e191cd455d7dcc264a762906b77e1b41a6ca2bad02baa062048abf`  
		Last Modified: Tue, 29 Mar 2022 13:27:15 GMT  
		Size: 4.2 MB (4209027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b22b1386f530e7fee07dd9f018f8076d82e0cd0fbdca127a40ea07409f52008`  
		Last Modified: Tue, 29 Mar 2022 13:27:14 GMT  
		Size: 1.7 KB (1651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c3c25ab25acfe04cdadb8caaeb67d72e2714e2fe8ee88de8341f673a79bf7f`  
		Last Modified: Tue, 29 Mar 2022 13:27:14 GMT  
		Size: 1.3 MB (1346168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630f1d9d0b94fc45eeb2f0c5be84db2475af934c99d43e7882822f03eac55ddb`  
		Last Modified: Tue, 29 Mar 2022 13:27:13 GMT  
		Size: 8.0 MB (8043552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fbc6770c3eb9d7ac46ed21380518743a917306d515324035750eabf469d36d`  
		Last Modified: Tue, 29 Mar 2022 13:27:12 GMT  
		Size: 1.0 MB (1025737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ddc1b1ef9aefd1d4d680d238c9a9a1f72c734667c0d58aae33319d52b3d74c`  
		Last Modified: Tue, 29 Mar 2022 13:27:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358dd17f48c0c9130aa57f25fabea42732d1d16077525d80b2b049245dcdd028`  
		Last Modified: Tue, 29 Mar 2022 13:27:12 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd1cf13c94953856de4abf3ff0f7e0b3af41f06eab60d57dfc16ac1038ae2b6`  
		Last Modified: Tue, 29 Mar 2022 13:27:21 GMT  
		Size: 87.8 MB (87799888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4283dcff5c4dcdd31de7cd87ec7345fda8e648bda98de413173888b26eb24a66`  
		Last Modified: Tue, 29 Mar 2022 13:27:10 GMT  
		Size: 9.5 KB (9530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7938a38c0b9ae000c810d88b095e4cbd3c288c29ac6f76732ca92c941c0a3615`  
		Last Modified: Tue, 29 Mar 2022 13:27:10 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05db87949cc9b0a7f8905647e507fead940fdd8ac85ffbe107e992e87a764471`  
		Last Modified: Tue, 29 Mar 2022 13:27:10 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7024c2908dfee3e17f979e2e2ef8998935c3cbbee81e14c49e75547cd779c5a7`  
		Last Modified: Tue, 29 Mar 2022 13:27:10 GMT  
		Size: 4.7 KB (4694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bullseye` - linux; 386

```console
$ docker pull postgres@sha256:e8c486f7d03eb4147c4d214bd12f60b896f9e1d10ffbe098f3e95f16cceda5cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139482694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66d58e8cc3e4a13fcfc490b1159c10c4aab574d7d6e997b22083beab27bdf8d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:18:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 11:18:17 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 11:18:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 11:18:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 11:18:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 29 Mar 2022 11:18:33 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 11:18:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 11:18:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 11:18:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 11:18:41 GMT
ENV PG_MAJOR=14
# Tue, 29 Mar 2022 11:18:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Tue, 29 Mar 2022 11:18:43 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Tue, 29 Mar 2022 11:32:01 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 29 Mar 2022 11:32:02 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 11:32:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 11:32:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 11:32:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 11:32:05 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 11:32:07 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:32:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 11:32:08 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 11:32:09 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 11:32:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1b48c2df933f48bc05387e474fc888b6b454d43a4ce228969d472ebfcb0d97`  
		Last Modified: Tue, 29 Mar 2022 12:40:00 GMT  
		Size: 4.6 MB (4606883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1e390ea4d727e0080f4867e8d7f998c54be27bb7f88620e7c4017726c99771`  
		Last Modified: Tue, 29 Mar 2022 12:39:58 GMT  
		Size: 1.6 KB (1644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749fefc8643c70f22d6dac623277500862d35219f2fe961fbac9b1c550cc9530`  
		Last Modified: Tue, 29 Mar 2022 12:39:59 GMT  
		Size: 1.4 MB (1385124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddf1c0eece1630acd9a3d3f1dfa88f55469da037316eb92c3e9a776b4fb5732`  
		Last Modified: Tue, 29 Mar 2022 12:39:58 GMT  
		Size: 8.0 MB (8043586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d86614993fee8b00cef6ea45e4046cb79ef561faa32ace4d1e46f670685644`  
		Last Modified: Tue, 29 Mar 2022 12:39:56 GMT  
		Size: 1.0 MB (1027776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5b635d32ce5d86be5686cf0dd2d0541992f56f3041e6c3fcd3e3b6d8276060`  
		Last Modified: Tue, 29 Mar 2022 12:39:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab642095e0b89b7bdcc28a641696207e612e3022e2acb187d82b3a624142060`  
		Last Modified: Tue, 29 Mar 2022 12:39:56 GMT  
		Size: 3.1 KB (3140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0255e8e64bc86460e552d15bd8da2caafad736366fcc61fcdd3b89a2740dba5e`  
		Last Modified: Tue, 29 Mar 2022 12:40:09 GMT  
		Size: 92.0 MB (92010371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014a0b777a55e37dbb953406e45bfabc0b270a73096fdd21b7d21ca522d0b60d`  
		Last Modified: Tue, 29 Mar 2022 12:39:54 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d178f9cd8e429984c0726102f0210cf980d419980623178f468ac7fdb28ed5`  
		Last Modified: Tue, 29 Mar 2022 12:39:54 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3726d230668a3b59ee71cd2ee4234b5c888c8a731a085feff5115d53ab1cc868`  
		Last Modified: Tue, 29 Mar 2022 12:39:54 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90c46169737c3f5f6939f3768b2bc568f7fbee28a60a374be837947381c2e38`  
		Last Modified: Tue, 29 Mar 2022 12:39:54 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:0dcdefab2b1be037127d938a80db17e862ecb49427372698339a0ca4798859fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132249578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ddf5672c2d045d39984812fd37c996d2b95bc94c399bbfeecaafe68debcb33d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 17 Mar 2022 08:53:04 GMT
ADD file:795ac4eba576bc4c995df2a18b10ce802ee8a05417cdc53f5aa09452ecf2e832 in / 
# Thu, 17 Mar 2022 08:53:08 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 13:21:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Mar 2022 13:21:56 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 18 Mar 2022 13:21:59 GMT
ENV GOSU_VERSION=1.14
# Fri, 18 Mar 2022 13:22:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Mar 2022 13:23:01 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 18 Mar 2022 13:23:04 GMT
ENV LANG=en_US.utf8
# Fri, 18 Mar 2022 13:23:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 13:23:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 18 Mar 2022 13:23:37 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 18 Mar 2022 13:23:40 GMT
ENV PG_MAJOR=14
# Fri, 18 Mar 2022 13:23:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 18 Mar 2022 13:23:45 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Fri, 18 Mar 2022 14:23:17 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 18 Mar 2022 14:23:25 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 18 Mar 2022 14:23:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 18 Mar 2022 14:23:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 18 Mar 2022 14:23:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 18 Mar 2022 14:23:46 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 18 Mar 2022 14:23:48 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Fri, 18 Mar 2022 14:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 14:23:55 GMT
STOPSIGNAL SIGINT
# Fri, 18 Mar 2022 14:23:59 GMT
EXPOSE 5432
# Fri, 18 Mar 2022 14:24:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4799d88734ae94287a665c0e14621a744706cfbe17a0cf27ae9b0cc630927b11`  
		Last Modified: Thu, 17 Mar 2022 10:43:20 GMT  
		Size: 29.6 MB (29639810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ec2ed639dba84d3cbabbacb1e071af830c7f28d1ce69239c0bfe1308f572c6`  
		Last Modified: Fri, 18 Mar 2022 17:51:07 GMT  
		Size: 4.2 MB (4196044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6f34c491bbee084842b5777d405fd742a31114da14ec4948eccd3df8bcb6e0`  
		Last Modified: Fri, 18 Mar 2022 17:51:02 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5f53bc45f3053707421b9dcc1dbb84ad61a4389df9dc870166e54d4d37b157`  
		Last Modified: Fri, 18 Mar 2022 17:51:04 GMT  
		Size: 1.3 MB (1297900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c700cea18921a0e15d8f66b49af05495b453602bdcd35feeb2a593c06426e37`  
		Last Modified: Fri, 18 Mar 2022 17:51:07 GMT  
		Size: 8.0 MB (8043925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc10f76f216534043fece8ecb35b6d9a489173f1d1fc24325b008221f1b110b8`  
		Last Modified: Fri, 18 Mar 2022 17:51:01 GMT  
		Size: 1.1 MB (1089183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adc71ab8e2e23fe65b2822ef03cc64dd862a9caaf894e1c31c67ef1970a5d18`  
		Last Modified: Fri, 18 Mar 2022 17:51:00 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef2c5b59ec298c84905a38626df46f3be6cef45702a28b590b2ef93f4abed66`  
		Last Modified: Fri, 18 Mar 2022 17:51:00 GMT  
		Size: 3.1 KB (3145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191325c448c021e910cb19fdba7f48098b00c410292d5824a6e1d8c3ba79780c`  
		Last Modified: Fri, 18 Mar 2022 17:51:55 GMT  
		Size: 88.0 MB (87963257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81ef2c77bef7f52ef05762aedab91f6a89f3e71f6f19b080d305f7fb5170f54`  
		Last Modified: Fri, 18 Mar 2022 17:50:57 GMT  
		Size: 9.5 KB (9543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d082decf89697135a1d1ccc58ef8b985176d118d277234f52a53dc8197df77a`  
		Last Modified: Fri, 18 Mar 2022 17:50:57 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b117baee9d8e871fc8ef4daf468b3adb62ead99730b928bfce988789a7cf7a2d`  
		Last Modified: Fri, 18 Mar 2022 17:50:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2c7c8c19a84cd60065cae653aba232dd66adf8e1216e0b9ef72bd95d619bb1`  
		Last Modified: Fri, 18 Mar 2022 17:50:57 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:2fecfaf1d8036abb5001ce7082e65648ad946df526dc45d6df45cc8cbce6a376
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146890056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65ca74945b1653e58225bb1240abcd1ed17369285a2beca3470e5514fc29096`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 05:27:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 05:27:48 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 29 Mar 2022 05:27:50 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 05:28:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 05:28:32 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 29 Mar 2022 05:28:35 GMT
ENV LANG=en_US.utf8
# Tue, 29 Mar 2022 05:28:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 05:28:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 29 Mar 2022 05:29:01 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 29 Mar 2022 05:29:03 GMT
ENV PG_MAJOR=14
# Tue, 29 Mar 2022 05:29:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Tue, 29 Mar 2022 05:29:08 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Tue, 29 Mar 2022 05:30:15 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 29 Mar 2022 05:30:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 29 Mar 2022 05:30:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 29 Mar 2022 05:30:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 29 Mar 2022 05:30:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 29 Mar 2022 05:30:45 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 29 Mar 2022 05:30:47 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 29 Mar 2022 05:30:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 05:30:52 GMT
STOPSIGNAL SIGINT
# Tue, 29 Mar 2022 05:30:55 GMT
EXPOSE 5432
# Tue, 29 Mar 2022 05:31:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d162321fceeb2e0a4748e729c0b263af174544c5651e2d602fc1da7473cbe5`  
		Last Modified: Tue, 29 Mar 2022 06:10:55 GMT  
		Size: 5.2 MB (5222952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f93fb033ee01298ec57cea5d0d33a4769d127b5c244156bc7ed2a86b6774e2a`  
		Last Modified: Tue, 29 Mar 2022 06:10:52 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d6aa761d145c50c561488248628dabcc82f77997b1c934fc48b70867442a64`  
		Last Modified: Tue, 29 Mar 2022 06:10:52 GMT  
		Size: 1.3 MB (1317569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03becbb5f9e5d219ac4edd8b17512b87b0b723fae2924f2456d62c412c2f3339`  
		Last Modified: Tue, 29 Mar 2022 06:10:52 GMT  
		Size: 8.0 MB (8045505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f84f1a83a9ce4c520e2d64e9b2dbc4a0d2dab17c53071e9c4bfea3704a7a97e`  
		Last Modified: Tue, 29 Mar 2022 06:10:51 GMT  
		Size: 1.4 MB (1420055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305183b206915bc145d09db49b29f6ce511608620c82fdb32d65e97ac8f1d45a`  
		Last Modified: Tue, 29 Mar 2022 06:10:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0041f4c48143628989e5661664c43e1348262356191468703d12f963e71fda0`  
		Last Modified: Tue, 29 Mar 2022 06:10:49 GMT  
		Size: 3.2 KB (3194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2988d94c3d97e74c0dc46f5cb37c041263265791ec2a2a15f7d9b463ec1eb39e`  
		Last Modified: Tue, 29 Mar 2022 06:11:03 GMT  
		Size: 95.6 MB (95581763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bfc2682e150550fbb7937afe518515bda2f8218a544084acc49a36cd06c51b`  
		Last Modified: Tue, 29 Mar 2022 06:10:46 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffaff6a0e8d70b6a0359bc88120269720d62a97ff33fade4c554b69acaea596`  
		Last Modified: Tue, 29 Mar 2022 06:10:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d36e00b9a71ea5a3ee9bf1e501ff5000596dfdaa21c3d311175f1bb0fba4d9`  
		Last Modified: Tue, 29 Mar 2022 06:10:46 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8475b7620c3f9abbd7ad13a7fd561b694d44be31ead41074e2f1a7d8867c83bf`  
		Last Modified: Tue, 29 Mar 2022 06:10:46 GMT  
		Size: 4.7 KB (4693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:a2ca85834f50b1ff9ad6b71c29b3111302b18e163df4f59145eb86c6eee2f517
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85130895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6095bc17ed41f847f08f09243690fe21844fe5500ef5788cf121ef93484ed3dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:57 GMT
ADD file:39c5e0d7a686abd19448ab3e6237d50955ae2187fc2b64289a08c2549352b8f1 in / 
# Tue, 29 Mar 2022 00:51:58 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 01:06:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 01:06:23 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 30 Mar 2022 01:06:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 30 Mar 2022 01:06:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 30 Mar 2022 01:06:55 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 30 Mar 2022 01:06:56 GMT
ENV LANG=en_US.utf8
# Wed, 30 Mar 2022 01:06:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 01:07:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 30 Mar 2022 01:07:05 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 30 Mar 2022 01:07:05 GMT
ENV PG_MAJOR=14
# Wed, 30 Mar 2022 01:07:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Wed, 30 Mar 2022 01:07:05 GMT
ENV PG_VERSION=14.2-1.pgdg110+1
# Wed, 30 Mar 2022 01:13:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 30 Mar 2022 01:13:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 30 Mar 2022 01:13:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 30 Mar 2022 01:13:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 30 Mar 2022 01:13:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 30 Mar 2022 01:13:57 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 30 Mar 2022 01:13:57 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Wed, 30 Mar 2022 01:13:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 01:13:57 GMT
STOPSIGNAL SIGINT
# Wed, 30 Mar 2022 01:13:57 GMT
EXPOSE 5432
# Wed, 30 Mar 2022 01:13:57 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ffb22bcde95509bb75f6dd2d69f3fdb5c7471727e4d720b31d92cd297582865c`  
		Last Modified: Tue, 29 Mar 2022 01:04:43 GMT  
		Size: 29.7 MB (29655426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ca697dcf68aa63d1bc830c7d8670adf8229c8b6b739926fe9080f7fdf5455a`  
		Last Modified: Wed, 30 Mar 2022 01:57:17 GMT  
		Size: 4.3 MB (4302353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4dc7cee6e6923d4117ce7fa66207b13274f4834c650103b6181f8eba6f3799`  
		Last Modified: Wed, 30 Mar 2022 01:57:17 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7cb5b68d46b21ca9f8e6560c3f41b779eade67eb22b1cc8f62cf22daa088f`  
		Last Modified: Wed, 30 Mar 2022 01:57:04 GMT  
		Size: 1.4 MB (1381466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ac7b0f24b6606317bdbfc7e20a5ce932aebab95b3138a27a4ff03cc7083a57`  
		Last Modified: Wed, 30 Mar 2022 01:56:56 GMT  
		Size: 8.1 MB (8099081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908999f2330b29c143736194404d59ac7c01818f34fd090ea89c0a825a4a580e`  
		Last Modified: Wed, 30 Mar 2022 01:56:56 GMT  
		Size: 1.2 MB (1237774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fefa9812fd71534271ba6a85e540b52726a1cec7dba15ec002f4fe5f7c2eef7`  
		Last Modified: Wed, 30 Mar 2022 01:56:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb43be03b957c5f110751711c47e86951c2671e216517c1d6f1db1aebfd12fa9`  
		Last Modified: Wed, 30 Mar 2022 01:56:56 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cec9ccbbf0573dbe066fceaf520e07fa6efcbf132724115acf4a76e899e3dc`  
		Last Modified: Wed, 30 Mar 2022 01:56:47 GMT  
		Size: 40.4 MB (40435080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b244ba9ed475e51338dd05402543bbad6e69715268b33cd69d5cba1bc77eaa`  
		Last Modified: Wed, 30 Mar 2022 01:56:40 GMT  
		Size: 9.5 KB (9538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5df32357edf22817212e0aef2fa43e6e0a0b8bc5fe65cc80f7ae3480e3cb566`  
		Last Modified: Wed, 30 Mar 2022 01:56:43 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4b48af860085c6125c51aa37e74d226aa9d56ca3b51b0ced0fe2e433b86cb`  
		Last Modified: Wed, 30 Mar 2022 01:56:43 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4fc1a81164ef25e71f0997071797cc2ddbfe82a876b9b36e7c3be69e9f2799`  
		Last Modified: Wed, 30 Mar 2022 01:56:39 GMT  
		Size: 4.7 KB (4695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
