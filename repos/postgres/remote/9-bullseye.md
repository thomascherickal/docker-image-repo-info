## `postgres:9-bullseye`

```console
$ docker pull postgres@sha256:4e2984b1b4d3cc17ce0dfd26165440c91987552c7cca43f831ff55adc1b3d33f
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

### `postgres:9-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:d795de9274ae9e8b0113719cab85087d22a5d9e07f8e161c0cd5e56b1fc95a04
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.9 MB (84879793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7bbf7c3c448f2129dc546df220c491690a90698b3e608e7b6c60370a8ca5e0d`
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
# Thu, 23 Sep 2021 23:58:39 GMT
ENV PG_MAJOR=9.6
# Thu, 23 Sep 2021 23:58:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Thu, 23 Sep 2021 23:58:39 GMT
ENV PG_VERSION=9.6.23-1.pgdg110+1
# Thu, 23 Sep 2021 23:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Sep 2021 23:58:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 23:58:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 23:58:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 23:58:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 23:58:57 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 23:58:57 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Thu, 23 Sep 2021 23:58:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Sep 2021 23:58:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 23:58:59 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 23:58:59 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 23:58:59 GMT
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
	-	`sha256:5f61322c3cd3fdbc7c2a865f13eb3c3c53bef5b66c9cdf1cadacf725298d273d`  
		Last Modified: Fri, 24 Sep 2021 00:03:06 GMT  
		Size: 39.1 MB (39141793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97da9df6ba3858368f80157cff72b8296a6022df09a44f32a5a36df6db4db0b4`  
		Last Modified: Fri, 24 Sep 2021 00:02:57 GMT  
		Size: 7.9 KB (7868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244d26ea128a3acc6b4d01b8f86f2466349cf4137b85f189021ab9a77a939a3d`  
		Last Modified: Fri, 24 Sep 2021 00:02:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792202cb614e06623258b3d66b40e43d05823b51042f9747201cd0f731422089`  
		Last Modified: Fri, 24 Sep 2021 00:02:57 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7382e674ab1ff5c3e08342ac0f61ecafee8caa814acfa51e0603a344b5b8513`  
		Last Modified: Fri, 24 Sep 2021 00:02:57 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006c9dc71fbdfbde80680c4012339a2b960c66bd7b5eefb9723eb26561de8a76`  
		Last Modified: Fri, 24 Sep 2021 00:02:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:704edc4dc0136249570ff617b0a8aba6edb272f1c1556fd026291e2a032e7baa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80629452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d73486bdae70ecf51369e3347e88c8e623f85e227bd3861e2545ea8518f0d149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:38 GMT
ADD file:da0067258fc1c6a50273e6b3b2673e88fad974a5a1fe4d5eecfeca2df1ff54b3 in / 
# Tue, 28 Sep 2021 01:50:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 04:21:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 04:21:51 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 04:21:52 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 04:22:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 04:22:38 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 04:22:39 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 04:22:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 04:22:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 04:22:55 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 08:02:32 GMT
ENV PG_MAJOR=9.6
# Tue, 28 Sep 2021 08:02:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 28 Sep 2021 08:02:33 GMT
ENV PG_VERSION=9.6.23-1.pgdg110+1
# Tue, 28 Sep 2021 08:24:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 08:24:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 08:24:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 08:24:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 08:24:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 08:24:26 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Sep 2021 08:24:27 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Tue, 28 Sep 2021 08:24:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 28 Sep 2021 08:24:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 08:24:29 GMT
STOPSIGNAL SIGINT
# Tue, 28 Sep 2021 08:24:30 GMT
EXPOSE 5432
# Tue, 28 Sep 2021 08:24:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:86f2b8be18fc44e8eb430e2c472979a79cda6eb6fa3add10cc8c5d8764eb90ac`  
		Last Modified: Tue, 28 Sep 2021 02:06:35 GMT  
		Size: 28.9 MB (28910670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d30eb8504c56819605185af701845341d8975e406423278405097f62af2306`  
		Last Modified: Tue, 28 Sep 2021 08:52:54 GMT  
		Size: 4.1 MB (4096354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a243eeeaa2c00737bdd6e98a1fa9a012a7867782cf48628d9ff8924d18b9f18`  
		Last Modified: Tue, 28 Sep 2021 08:52:52 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11403c7ba143852cedde2cb5fc5d9667ab0334c046a7c9ebc8c7850e05fb9c83`  
		Last Modified: Tue, 28 Sep 2021 08:52:52 GMT  
		Size: 1.4 MB (1409777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f8edfacdf52bfedbf204f96cfb85a0e19c8565f7466afdffca94537cd94624`  
		Last Modified: Tue, 28 Sep 2021 08:52:57 GMT  
		Size: 8.0 MB (8045267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823170a97ccf0c83730d7cc699ed2b8cc784fa3a3a434fca8d95389d5a47dee3`  
		Last Modified: Tue, 28 Sep 2021 08:52:50 GMT  
		Size: 439.8 KB (439807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b92b828995d7ff6cb1b2a36baf84eadb6717f6070738cd8e1f2e79abdb34e6`  
		Last Modified: Tue, 28 Sep 2021 08:52:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a0b55cf0d04e78b149e19f243e52ab82558abba6430057c63594f69cc4f8b0`  
		Last Modified: Tue, 28 Sep 2021 08:52:50 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332cb4530817b0d8435520c9d0e733e6aadefec3b9b7310e993361be4966846e`  
		Last Modified: Tue, 28 Sep 2021 09:00:25 GMT  
		Size: 37.7 MB (37709855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca3b551abcbb25eaa40ebb1f4ff684e39be6a77192a7b51d66c22cdc0be2942`  
		Last Modified: Tue, 28 Sep 2021 08:59:57 GMT  
		Size: 7.9 KB (7873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b284ebc7c49ab6f2c574423dcd21502065a3227d2497f7e461e872359f7644a`  
		Last Modified: Tue, 28 Sep 2021 08:59:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c01ec4330fefbc07f82e034ae491cad6b7b845d947dcd4977c418b14761ddb3`  
		Last Modified: Tue, 28 Sep 2021 08:59:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b7fdabbd4404177c100a5a5466bc84ae217f1f04b57974f1a994eb94dacb2d`  
		Last Modified: Tue, 28 Sep 2021 08:59:57 GMT  
		Size: 4.4 KB (4405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14363722e982b1058ff26f3ffa91aaf7e0324ecf473f989405f4827111f44115`  
		Last Modified: Tue, 28 Sep 2021 08:59:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:964d9bebbca4afc008727bf9eb4f1c6a8988270627cec6b01300a1bab570cef3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83264464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06820d891b46e5f1f07a09caded5b2371e76106eae289de788c7d6b4de26f0ae`
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
# Fri, 24 Sep 2021 01:30:00 GMT
ENV PG_MAJOR=9.6
# Fri, 24 Sep 2021 01:30:00 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 24 Sep 2021 01:30:01 GMT
ENV PG_VERSION=9.6.23-1.pgdg110+1
# Fri, 24 Sep 2021 01:30:15 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 01:30:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 01:30:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 01:30:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 01:30:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 01:30:17 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 01:30:18 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Fri, 24 Sep 2021 01:30:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Sep 2021 01:30:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 01:30:19 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 01:30:19 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 01:30:19 GMT
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
	-	`sha256:2a9b0c24aa380c06fa1bb1bbc10d1f79104240692f34a711bedbf4d0022f318a`  
		Last Modified: Fri, 24 Sep 2021 01:35:49 GMT  
		Size: 38.9 MB (38902207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a8a835fff6f03fd9c797d472b0303f558271930a2c70522198f6e00eae4ed4`  
		Last Modified: Fri, 24 Sep 2021 01:35:40 GMT  
		Size: 7.9 KB (7867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859422a772b0b7c67b0a0e45a57db9a5d59f9647a0de38eabc0b9891b1750651`  
		Last Modified: Fri, 24 Sep 2021 01:35:40 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c46f22efe9d2134adada1b42942196af72a986a9590e6125cad1b58943f5b03`  
		Last Modified: Fri, 24 Sep 2021 01:35:40 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4dd1e0c45fab89df1b51610d04e6471d256506a05ad3dad4c94c164b738f9fd`  
		Last Modified: Fri, 24 Sep 2021 01:35:40 GMT  
		Size: 4.4 KB (4399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676f19115fdf4194f959b15a6383fb588bb15856b749f58c85db349e01a178ff`  
		Last Modified: Fri, 24 Sep 2021 01:35:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:32e4e7818041a025daebf22e88b25bcb0c6bddfb40884f6ce43c2ace915baa58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.4 MB (86416750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4922e46226772660d98afd9751780fd2086756c80ec12e4409aaccb267757c1a`
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
# Fri, 24 Sep 2021 00:17:01 GMT
ENV PG_MAJOR=9.6
# Fri, 24 Sep 2021 00:17:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 24 Sep 2021 00:17:02 GMT
ENV PG_VERSION=9.6.23-1.pgdg110+1
# Fri, 24 Sep 2021 00:29:12 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 00:29:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 00:29:15 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 00:29:15 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 00:29:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 00:29:16 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 00:29:17 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Fri, 24 Sep 2021 00:29:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Sep 2021 00:29:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 00:29:19 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 00:29:19 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 00:29:20 GMT
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
	-	`sha256:50b3f81a860d90033805a19fa28b0bed391a0775d3ced28c11a6772e531ecfd4`  
		Last Modified: Fri, 24 Sep 2021 00:37:15 GMT  
		Size: 39.3 MB (39292471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0d140144ad212b9733a0bf04299e42e9f6515e36458adb66672c0963f5cd84`  
		Last Modified: Fri, 24 Sep 2021 00:37:03 GMT  
		Size: 7.9 KB (7871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9396dae8fffcc99eec3ba12f8bdf6d04961ac6c5c13788633b742f4f04ef7d5`  
		Last Modified: Fri, 24 Sep 2021 00:37:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1380f1474c833738c230fc42ae578432d45de29609aa44a5f7b043d1bfa24af3`  
		Last Modified: Fri, 24 Sep 2021 00:37:03 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19aca784103d40acb23d28343fd90bc22ae7404e2f22cffa11d6e9826bb81d16`  
		Last Modified: Fri, 24 Sep 2021 00:37:03 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d699d4fdc49f6642b79e31ead169ec7545ac4afa4569da70ae1340e429463dcd`  
		Last Modified: Fri, 24 Sep 2021 00:37:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:1e4d2dd9d761dcfcd82f65921b54fde119b8eecfbe7a1651c9d4cf5a6f503a3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.9 MB (81899564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0fd350b382a4371efaecf86c528c4e14778c1071a8bd8c4b1b6507437209ff2`
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
# Fri, 24 Sep 2021 02:56:46 GMT
ENV PG_MAJOR=9.6
# Fri, 24 Sep 2021 02:56:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 24 Sep 2021 02:56:47 GMT
ENV PG_VERSION=9.6.23-1.pgdg110+1
# Fri, 24 Sep 2021 03:31:02 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 03:31:05 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 03:31:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 03:31:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 03:31:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 03:31:10 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 03:31:10 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Fri, 24 Sep 2021 03:31:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Sep 2021 03:31:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 03:31:13 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 03:31:13 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 03:31:14 GMT
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
	-	`sha256:cfe3445b81f7c4db20dda840714b0ed602ab0ace2a12aea75c4a19a71ea688ee`  
		Last Modified: Fri, 24 Sep 2021 03:37:54 GMT  
		Size: 38.0 MB (38029307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0573b817433efe95c44edc3f7dcc7d0c8cd555797fca39a9e24622a38ab56a0`  
		Last Modified: Fri, 24 Sep 2021 03:37:24 GMT  
		Size: 7.9 KB (7870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c985c5f1840adda627fcfbfbaba0c6c46106659437ca03495908b6f41faf7792`  
		Last Modified: Fri, 24 Sep 2021 03:37:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ea71976e0d561288e399059f95c692c7a01eb585926f65ef7736609f0dda61`  
		Last Modified: Fri, 24 Sep 2021 03:37:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635a2b5454164a118f01da279fba64ed4997d2dd073f3bf770db68f266523299`  
		Last Modified: Fri, 24 Sep 2021 03:37:24 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e003f87e9705e22479a27bbdd47f40f500a0ee2f3cc405f1cf22dafddd43b4c8`  
		Last Modified: Fri, 24 Sep 2021 03:37:24 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:bc22a345dbdfa29d7df1f4526dda0cd38896971e66045159f7fff7b40fd3f608
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91116606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:657d02e9776d1400709b8d8560ac500680d86df0c9db2fb01998062f7bc03a45`
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
# Fri, 24 Sep 2021 07:12:59 GMT
ENV PG_MAJOR=9.6
# Fri, 24 Sep 2021 07:13:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 24 Sep 2021 07:13:08 GMT
ENV PG_VERSION=9.6.23-1.pgdg110+1
# Fri, 24 Sep 2021 07:15:17 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 07:15:41 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 07:15:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 07:16:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 07:16:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 07:16:30 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 07:16:32 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Fri, 24 Sep 2021 07:16:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Sep 2021 07:16:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 07:17:20 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 07:17:29 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 07:17:40 GMT
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
	-	`sha256:32f853f0d582d2b8335780b171969d1a46f152c25eef0dbd1c444875d22f729c`  
		Last Modified: Fri, 24 Sep 2021 07:22:58 GMT  
		Size: 40.7 MB (40736728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57de2d12ede6204d6bf16ebda8216538eead28fa10440d6badc5303bfa4a1446`  
		Last Modified: Fri, 24 Sep 2021 07:22:47 GMT  
		Size: 7.9 KB (7880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e87e6268603078ad1759449e006e36dd78841c890aba53fab00f870780e071`  
		Last Modified: Fri, 24 Sep 2021 07:22:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141df6e63f67accf889a10464db361106fdae0cebe3fa8d59f50a8165a2227a8`  
		Last Modified: Fri, 24 Sep 2021 07:22:47 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abc1d4c965a3c157788e4194a3b45163f2b940a62c9496b04e97962d9d0e177`  
		Last Modified: Fri, 24 Sep 2021 07:22:47 GMT  
		Size: 4.4 KB (4400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370a26bfc2e0c7ed77d79603926b3d4ddfd658c47fec7966ebb668204db0f29`  
		Last Modified: Fri, 24 Sep 2021 07:22:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:e5d3d998c7752b7f62bb7cd37fef5a343e3fdd2c3e058907db8ccdea7d8fe2d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83180569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bd5d61afa70d8d4fe895dba5f15326773123605f77b4c7a63c084509836ed76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:57 GMT
ADD file:2daa8824c30440336bc6ea1448af03234d491ad7c0d0cac917cae5eb54c315fc in / 
# Tue, 28 Sep 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:36:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:36:39 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 02:36:39 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 02:36:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 02:36:51 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 02:36:51 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 02:36:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:36:55 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 02:37:01 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 03:20:02 GMT
ENV PG_MAJOR=9.6
# Tue, 28 Sep 2021 03:20:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 28 Sep 2021 03:20:02 GMT
ENV PG_VERSION=9.6.23-1.pgdg110+1
# Tue, 28 Sep 2021 03:25:48 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 03:25:50 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 03:25:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 03:25:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 03:25:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 03:25:51 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Sep 2021 03:25:52 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Tue, 28 Sep 2021 03:25:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 28 Sep 2021 03:25:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 03:25:52 GMT
STOPSIGNAL SIGINT
# Tue, 28 Sep 2021 03:25:52 GMT
EXPOSE 5432
# Tue, 28 Sep 2021 03:25:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e8e2938f4df931c46d7575f0b7bad5bc357277fc3e132b720e704ac7a4d1c9ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:01 GMT  
		Size: 29.7 MB (29650795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec9abc08cf3416245d8969464ffc09bd7d906b53ccb79e8a871fa76ff53345`  
		Last Modified: Tue, 28 Sep 2021 03:27:46 GMT  
		Size: 4.3 MB (4302149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76b20cabec1e9c13874c288a755ecb8be19bff7cde71239da194df4f8c4f8`  
		Last Modified: Tue, 28 Sep 2021 03:27:45 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df8fb2145140202ec944f2eec276009afed7dac0058e18627ab9092ec4b32b`  
		Last Modified: Tue, 28 Sep 2021 03:27:46 GMT  
		Size: 1.4 MB (1437294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aa9ea8f851bf56a4b0a02d952d04b16d85fe90c215c95bee50946b3c3b371`  
		Last Modified: Tue, 28 Sep 2021 03:27:45 GMT  
		Size: 8.1 MB (8098989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beb5a03c6f20aa530f94ace58ca4c26cab6b8a9c07ff8e60584b9bb75e55cf`  
		Last Modified: Tue, 28 Sep 2021 03:27:44 GMT  
		Size: 438.2 KB (438229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9ca31c5b54e8da36d434096006a112bfca32e5098d8af92803146e54f2cd83`  
		Last Modified: Tue, 28 Sep 2021 03:27:44 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc2177f334345af5c565c7ab75adf6a52e25583a1ddb3dea012692f4476b9c7`  
		Last Modified: Tue, 28 Sep 2021 03:27:44 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e094399b8b58f962dd29a737fe46e6b62674de6a1af63ed643e13b5c39ebd5e`  
		Last Modified: Tue, 28 Sep 2021 03:29:44 GMT  
		Size: 39.2 MB (39235385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58eea496a293b9690d1faa5e9befb3e3208b2f47d0ddd125bbee27e5c37f022`  
		Last Modified: Tue, 28 Sep 2021 03:29:38 GMT  
		Size: 7.9 KB (7872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f428fc30b04dd7a4fc70c1eb1d70ee67e6d6627cb593cd76ccea1fca692420a6`  
		Last Modified: Tue, 28 Sep 2021 03:29:37 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94ce4886c432aaa8b6c0dfb463f430726174c9763b72bf765ddfd78b9acfb7a`  
		Last Modified: Tue, 28 Sep 2021 03:29:37 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8df6b3ad1a157e2daeec139bdf9b8d6134be2b2f7e00a42cdc1e8893c596f99`  
		Last Modified: Tue, 28 Sep 2021 03:29:37 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652afeb740bc88b1b46f4e24982786744ce52d2ffcca594e73f31237d67d8a44`  
		Last Modified: Tue, 28 Sep 2021 03:29:37 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
