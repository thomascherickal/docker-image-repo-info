## `postgres:10-bullseye`

```console
$ docker pull postgres@sha256:8608f59eef6fa08f5f55d55f8a86b26cb45f1b65ee2601000cd3f979781d1b4a
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

### `postgres:10-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:b2634e2b0da94dd5e0a062520f44d8208c2fba4f53c8d1f3fa83262b18fe8e67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84514877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50ae2a57a6259d362269d7c8e31f92969869b49640045b33548c32851225fdf`
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
# Thu, 23 Sep 2021 23:58:03 GMT
ENV PG_MAJOR=10
# Thu, 23 Sep 2021 23:58:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Thu, 23 Sep 2021 23:58:03 GMT
ENV PG_VERSION=10.18-1.pgdg110+1
# Thu, 23 Sep 2021 23:58:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Sep 2021 23:58:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 23:58:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 23:58:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 23:58:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 23:58:24 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 23:58:25 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Thu, 23 Sep 2021 23:58:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Sep 2021 23:58:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 23:58:26 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 23:58:26 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 23:58:26 GMT
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
	-	`sha256:73809fa29323a134fe82cf208a2e82ef375de83e1f4f4b1f84f7bbc9bb7eb685`  
		Last Modified: Fri, 24 Sep 2021 00:02:42 GMT  
		Size: 38.8 MB (38776678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f872e6275396b915f06c919a0ad13db3991a911bf42bcd649376df3f1026e58`  
		Last Modified: Fri, 24 Sep 2021 00:02:33 GMT  
		Size: 8.1 KB (8073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9e66ba90ccf1e5c2ce75b580533b3027990510f804143bb898a4ed5eaeb48f`  
		Last Modified: Fri, 24 Sep 2021 00:02:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63655df8234a8e40dc4f4303bc3eca1ff4fad1310190a68355d4b463b21bbee7`  
		Last Modified: Fri, 24 Sep 2021 00:02:33 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf96eec4b74f2c2e171bb723f8b4013e6d8bfcbdc21bf3bc6e835543310dfe`  
		Last Modified: Fri, 24 Sep 2021 00:02:34 GMT  
		Size: 4.4 KB (4398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b3679cee853d4077cb80490a8926a7cc5991099dce107a5d069dfb7750ec7d`  
		Last Modified: Fri, 24 Sep 2021 00:02:33 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:4c9b007aba61c28d2413de8db43678affeaea61897922574d4034b6eff708ec3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.2 MB (80246512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b381a54b2741a37948ef59c0ff278d9f8a7d9af0b2b86a9df1b999ac14cd1434`
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
# Fri, 24 Sep 2021 05:27:51 GMT
ENV PG_MAJOR=10
# Fri, 24 Sep 2021 05:27:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Fri, 24 Sep 2021 05:27:52 GMT
ENV PG_VERSION=10.18-1.pgdg110+1
# Fri, 24 Sep 2021 05:50:32 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 05:50:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 05:50:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 05:50:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 05:50:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 05:50:39 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 05:50:39 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 24 Sep 2021 05:50:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Sep 2021 05:50:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 05:50:42 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 05:50:42 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 05:50:43 GMT
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
	-	`sha256:4918cb307a6954ef3fe2e1913cdb4fa75178aeb586a8fa8daf89a0854215c854`  
		Last Modified: Fri, 24 Sep 2021 06:21:36 GMT  
		Size: 37.3 MB (37326677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93153026e0bd6c216c7003edd2400c58af1b6d53116a742a2fb53544f2638377`  
		Last Modified: Fri, 24 Sep 2021 06:21:07 GMT  
		Size: 8.1 KB (8076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9425d2736a3aaa9230f3360cf11ce32fe7abe790c151175765c0bcc9c1495d5`  
		Last Modified: Fri, 24 Sep 2021 06:21:08 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e58a258d11d4ed6a03100cf81d687274642c3ae31b12231cd952f8f0eb94962`  
		Last Modified: Fri, 24 Sep 2021 06:21:08 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895d7be1addecb259207e55bc80709c8d4ce7a8cabff6571c73e299c016f7fb0`  
		Last Modified: Fri, 24 Sep 2021 06:21:08 GMT  
		Size: 4.4 KB (4400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b8f879eaff19e6126668333b5ef0d0078da645a9dba04fc7105e211c88c842`  
		Last Modified: Fri, 24 Sep 2021 06:21:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:890a73f45b6cf05c91eebfd5a3af335e2aee3f3b2bb0b7c7cb4d95822afa51a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82884297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7714b323dfaeea0b9ba7b7197f31af45a8eedaea477419736ed9c91bbb9465d`
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
# Fri, 24 Sep 2021 01:29:27 GMT
ENV PG_MAJOR=10
# Fri, 24 Sep 2021 01:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Fri, 24 Sep 2021 01:29:27 GMT
ENV PG_VERSION=10.18-1.pgdg110+1
# Fri, 24 Sep 2021 01:29:40 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 01:29:41 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 01:29:41 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 01:29:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 01:29:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 01:29:43 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 01:29:43 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 24 Sep 2021 01:29:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Sep 2021 01:29:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 01:29:44 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 01:29:44 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 01:29:44 GMT
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
	-	`sha256:7df320196f616453a536e06b3bdaa19ea371f8484e470b5676d23e7bbda98f16`  
		Last Modified: Fri, 24 Sep 2021 01:35:22 GMT  
		Size: 38.5 MB (38521830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664282f7f208b37c2507c339df8881c36470eca6c2ecd71bde7538f93b31198b`  
		Last Modified: Fri, 24 Sep 2021 01:35:13 GMT  
		Size: 8.1 KB (8074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beb20bc452bc0b20dccfc8ddc01e772337ad62735654d70b413b7a1d8ace848`  
		Last Modified: Fri, 24 Sep 2021 01:35:13 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57562df23779ce86acda9520d46a38de29a09ee6f118d99916882af6079ead6d`  
		Last Modified: Fri, 24 Sep 2021 01:35:14 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b89aacbd737bd013f8ff2f45e20906101722c6a0e3c6caba6dcf6fb70164c9`  
		Last Modified: Fri, 24 Sep 2021 01:35:13 GMT  
		Size: 4.4 KB (4400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250f30763511cb4d2f8f635592a4d2ee4bf5c9e640474f6fe077d21396d7d7aa`  
		Last Modified: Fri, 24 Sep 2021 01:35:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:ad48d55b9640e9cffd1a4b8321ebce683008860c9d7773d5059ce29f3ad04b69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86079795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d197ccd0c7501ca62cbb58a5f152c358d53c58643fc4ebc755b3b5a18b6ae9`
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
# Fri, 24 Sep 2021 00:03:56 GMT
ENV PG_MAJOR=10
# Fri, 24 Sep 2021 00:03:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Fri, 24 Sep 2021 00:03:57 GMT
ENV PG_VERSION=10.18-1.pgdg110+1
# Fri, 24 Sep 2021 00:16:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 00:16:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 00:16:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 00:16:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 00:16:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 00:16:26 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 00:16:27 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 24 Sep 2021 00:16:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Sep 2021 00:16:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 00:16:29 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 00:16:29 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 00:16:29 GMT
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
	-	`sha256:17a912b6c19edd465a0a003df061cd8fbb5cd94d8404fe2a6b85b0d210165097`  
		Last Modified: Fri, 24 Sep 2021 00:36:41 GMT  
		Size: 39.0 MB (38955311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3f8af51418985501ae28a48fe36d88ef871b961f1fc28e7ca712eefde7b374`  
		Last Modified: Fri, 24 Sep 2021 00:36:30 GMT  
		Size: 8.1 KB (8077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79bac5c86d96d6aaadaf3b6b6bdffecfcf0d1b138d8ad120615ca59f282b578`  
		Last Modified: Fri, 24 Sep 2021 00:36:30 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771e29d94bdf9654e74f694b499e69d783947313c2c32055910fc5c9317d7084`  
		Last Modified: Fri, 24 Sep 2021 00:36:30 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61f43e2e18cae7d7dba0b955ae6f305cf14a7d9bdad1c6a76f0390a9ca3617`  
		Last Modified: Fri, 24 Sep 2021 00:36:30 GMT  
		Size: 4.4 KB (4402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb6cb731ff9d2afd2d5a022888e2259843b628ea42c6c17e843eafde0265b28`  
		Last Modified: Fri, 24 Sep 2021 00:36:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:65d17bffc280702e6ca749bad2f141d8e765190dbe010334d9cc43f4791a9273
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81509255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a77bdc8826f1c73c1df0d6114f6e88d819d4529c2c59529eb83bcb86f1a27c9`
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
# Fri, 24 Sep 2021 02:20:52 GMT
ENV PG_MAJOR=10
# Fri, 24 Sep 2021 02:20:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Fri, 24 Sep 2021 02:20:53 GMT
ENV PG_VERSION=10.18-1.pgdg110+1
# Fri, 24 Sep 2021 02:56:18 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 02:56:20 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 02:56:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 02:56:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 02:56:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 02:56:25 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 02:56:25 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 24 Sep 2021 02:56:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Sep 2021 02:56:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 02:56:28 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 02:56:28 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 02:56:29 GMT
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
	-	`sha256:17442f7a0d5ffc66028ec36a0679a84ce18e7cc1c5f7ba3baea542f21511caff`  
		Last Modified: Fri, 24 Sep 2021 03:37:14 GMT  
		Size: 37.6 MB (37638790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43c2c10f5379f9bb6a7be38fed6ebbdde20176d45fc83126265d0fbecfd0c3a`  
		Last Modified: Fri, 24 Sep 2021 03:36:43 GMT  
		Size: 8.1 KB (8079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e935d317260778c6866d4f2d39af9c89a6162dd9d2b0b7e3b639fb479e4874ff`  
		Last Modified: Fri, 24 Sep 2021 03:36:43 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7188c22a97588f3439c6a68667825d8663abde04ef21366ec552f9b1c135da`  
		Last Modified: Fri, 24 Sep 2021 03:36:43 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd77454527c2ec1baef4e0f053acb46d9ff4a4a2dc41a702a521141b99125d4`  
		Last Modified: Fri, 24 Sep 2021 03:36:43 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef00aab6fae3a21d2ad32595c3f35a2c666daf37c081da7a8d9f71c510abdf4`  
		Last Modified: Fri, 24 Sep 2021 03:36:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:59302e07b6934b86052305563da85d11b26afd2d0e317ee35a5b195b85b43365
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90781138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e33d97ad174ec5b4f3b6a33e80541234455ff0c09dc7225d40ca876d935045c2`
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
# Fri, 24 Sep 2021 07:09:24 GMT
ENV PG_MAJOR=10
# Fri, 24 Sep 2021 07:09:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Fri, 24 Sep 2021 07:09:33 GMT
ENV PG_VERSION=10.18-1.pgdg110+1
# Fri, 24 Sep 2021 07:11:01 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Sep 2021 07:11:20 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Sep 2021 07:11:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Sep 2021 07:11:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Sep 2021 07:11:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Sep 2021 07:11:58 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Sep 2021 07:12:00 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Fri, 24 Sep 2021 07:12:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 24 Sep 2021 07:12:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 07:12:19 GMT
STOPSIGNAL SIGINT
# Fri, 24 Sep 2021 07:12:26 GMT
EXPOSE 5432
# Fri, 24 Sep 2021 07:12:33 GMT
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
	-	`sha256:37435aff1c7af0bf2935c96ab1bddcc8d5ba25de8e4cafb5968ab804e4554624`  
		Last Modified: Fri, 24 Sep 2021 07:22:32 GMT  
		Size: 40.4 MB (40401053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a96a9293bc10b480f558019aa0a1f0ed83405d6ffab5ed2bc202567b176c77`  
		Last Modified: Fri, 24 Sep 2021 07:22:21 GMT  
		Size: 8.1 KB (8084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfd6b016b355217d4260caa35e87afc3dc9a5d036a111796d23ad9995e516ff`  
		Last Modified: Fri, 24 Sep 2021 07:22:22 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9febcbd78d9c628366c6d2d6a3518f9b69c05218e4d9740747827423a124c958`  
		Last Modified: Fri, 24 Sep 2021 07:22:21 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d484a342206f590a690ec99d4444f3ba2eb4ae709ef2f7a4c2b734b889b824b`  
		Last Modified: Fri, 24 Sep 2021 07:22:21 GMT  
		Size: 4.4 KB (4403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8d37c38ee2158a03a91b65412f7b47541dc6d2cc2e2bc4b85c6a20d7e8137f`  
		Last Modified: Fri, 24 Sep 2021 07:22:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:10-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:8cccfb0d171ed16fb6c5f1c72c465a81f199fac7b94245ff05c798dccb747327
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82813687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:553d0785ee45add5e7bd236a2c5e7c98b71596aeeba0eb0c74789c493afa1580`
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
# Thu, 23 Sep 2021 23:19:30 GMT
ENV PG_MAJOR=10
# Thu, 23 Sep 2021 23:19:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/10/bin
# Thu, 23 Sep 2021 23:19:30 GMT
ENV PG_VERSION=10.18-1.pgdg110+1
# Thu, 23 Sep 2021 23:25:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Sep 2021 23:25:58 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Sep 2021 23:25:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Sep 2021 23:25:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Sep 2021 23:25:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Sep 2021 23:25:59 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 23 Sep 2021 23:25:59 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Thu, 23 Sep 2021 23:26:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 23 Sep 2021 23:26:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 23:26:00 GMT
STOPSIGNAL SIGINT
# Thu, 23 Sep 2021 23:26:00 GMT
EXPOSE 5432
# Thu, 23 Sep 2021 23:26:00 GMT
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
	-	`sha256:f1c36e0e0628857e4e599981c11b514e3f2117207052401822068c87d57714f6`  
		Last Modified: Thu, 23 Sep 2021 23:37:00 GMT  
		Size: 38.9 MB (38868469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02cbf30ee405042e90ffb9925ab4b16e180121cb027c1a6dcd50f28cb9c942d`  
		Last Modified: Thu, 23 Sep 2021 23:36:53 GMT  
		Size: 8.1 KB (8075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d011e6d3c482ba32e35ed7c151c89125516ef38199cdb1f51ad8338619f1e53`  
		Last Modified: Thu, 23 Sep 2021 23:36:53 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b6404aa504db74b59a74fd1f2d5996c3d9c8df82a7cac0ace044ff2ecd9484`  
		Last Modified: Thu, 23 Sep 2021 23:36:54 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4151c30995fe9df3f7d7c14a9994075c09813568982e78ce87d2d77b1f8d313d`  
		Last Modified: Thu, 23 Sep 2021 23:36:53 GMT  
		Size: 4.4 KB (4401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dbfed7fbb710e48eab7813694c6cb37f7d838ac34f5f856b0682ef85074053`  
		Last Modified: Thu, 23 Sep 2021 23:36:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
